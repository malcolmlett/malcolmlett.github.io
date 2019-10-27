What actually happens in order to execute a thought process from start to finish? This page answers that threw some detailed examples.

## Solve "3 + 8"
The processing of user command "3 + 8" occurs as follows:

| Step | Processor | Description |
|---|---|---|
| 1 | User request                        | "3 + 8" enters input sense |
| 2 | RequestCommandInterceptor           | Emits TextRequestEvent to WM, holding text "3 + 8" |
| 3 | ExpressionAndEquationParseProcessor | Detects TextRequestEvent. Pre-programmed to "just know" how to parse expressions. Emits PerceptEvent containing parsed expression as a syntax tree |
| 4 | ExpressionEvaluationProcessor       | Detects PerceptEvent flagged with pre-programmed Expression concept. Pre-programmed to "just know" how to evaluate expressions. Emits PerceptEvent containing resultant number, flagged as a result |
| 5 | ExpressionResponseProcessor         | Detects result PerceptEvent and presence of a user request. Emits ActionEvent with text of response "11" |
| 6 | SpeakActionProcessor                | Detects ActionEvent. "Speaks" response text |

## Solve "3 + ? = 8"
_**Note: this is a work-in-progress.**_

The processing of user command "3 + ? = 8", without user interaction to help the process, occurs over about 3 stages, as follows:

| Step | Processor | Description |
|---|---|---|
| 1.0 | User request                        | "3 + ? = 8" |
| 1.0 | RequestCommandInterceptor           | Emits TextRequestEvent to WM |
| 1.1 | ExpressionAndEquationParseProcessor | Emits PerceptEvent with partially parsed expression |
| 1.2 | EquationEvaluationProcessor         | Does nothing. Unable to process |
| 2.0 | StuckThoughtInterceptor             | Emits StuckThoughtEvent |
| 2.1 | FindMatchingConceptProcessor        | Assumes need to find concepts due to StuckThought, emits MemorySearchRequest |
| 2.2 | LongTermMemorySearchProcessor       | Searches LTM, emits MemoryEvent |
| 2.3 | FindMatchingConceptProcessor        | Assumes need to find concepts due to StuckThought, finds one or more in WM, so stops |
| 2.4 | (...)                               | What selects one of the concepts to try against? First cut: for now just pick single greedy option, in both ConceptInferenceProcessor and GapFillingProcessor. |
| 2.5 | ConceptInferenceProcessor           | Attempts to infer an identification of concept for '?' based on matching against concepts in WM. Emits a Percept if it discovers something better than what's already present. Emit new Percept theorising that '?' is a number. |
| 2.6 | GapFillingProcessor                 | Attempts to fill gap in partially parsed expression using concept/concepts available in WM, including any inferred concepts if present. Emit new Equation Percept, with '?' tagged as a number. |
| 2.7 | EquationEvaluationProcessor         | Needs to kick in a try again against new equation percept. Will fail once again. |
| 3.0 | StuckThoughtInterceptor             | Emits StuckThoughtEvent|
| 3... | (...)                              | [WIP] Now start employing strategies to guess at number value of '?' |
| x.x | FindMatchingConceptProcessor        | [WIP] Last found concept(s) not good enough, tries again |
