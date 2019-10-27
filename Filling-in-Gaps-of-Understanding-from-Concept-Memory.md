## Problem
How to solve "3 + ? = 8" without having previously been trained to cope with such expressions, and without knowing anything about what '?' might be? And how can it solve that without any help?

## Solution
...to be scanned...

## Review of Processors
The processing of "3 + ? = 8" currently occurs via the following steps:

| Step | Processor | Description |
|---|---|---|
| 0 | (interceptor)                       | TextRequestEvent present |
| 1 | ExpressionAndEquationParseProcessor | Emits PerceptEvent with partially parsed expression |
| 2 | EquationEvaluationProcessor         | Fails to process |
| 3 | (interceptor)                       | StuckThoughtEvent present |
| 4 | FindMatchingConceptProcessor        | Assumes need to find concept due to StuckThought, emits MemorySearchRequest |
| 5 | LongTermMemorySearchProcessor       | Searches LTM, emits MemoryEvent |
| 6 | FindMatchingConceptProcessor        | Assumes need to find concept due to StuckThought, finds in WM, so stops |
| 7 | 