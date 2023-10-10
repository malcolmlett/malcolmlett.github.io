---
title: Filling in Gaps of Understanding from Concept Memory
layout: wiki
parent: Wiki
---

## Problem
How to solve "3 + ? = 8" without having previously been trained to cope with such expressions, and without knowing anything about what '?' might be? And how can it solve that without any help?

## Solution
...to be scanned...

## High Level Description of Solution
We're automating a sequence that could otherwise have been instructor led, but still emulate a lot of interesting things:
1. Solve "3 + ? = 8"
2. Calculator: What's '?'?
3. It's a number.
4. Try a number.
5. Calculator: "3 + <picks a random number> = 8 => false"
6. Keep trying.
7. Calculator: keeps trying for a short period, gives up.
8. Keep trying.
9. Calculator: adjusts perseverance.
10. Calculator: keeps trying until it succeeds.
11. Calculator: "3 + 5 = 8".

## Review of Processor Steps
The processing of "3 + ? = 8" currently occurs via the following steps, broken into stages:

| Step | Processor | Description |
|---|---|---|
| 1.0 | (interceptor)                       | TextRequestEvent present |
| 1.1 | ExpressionAndEquationParseProcessor | Emits PerceptEvent with partially parsed expression |
| 1.2 | EquationEvaluationProcessor         | Fails to process |
| 2.0 | (interceptor)                       | StuckThoughtEvent present |
| 2.1 | FindMatchingConceptProcessor        | Assumes need to find concepts due to StuckThought, emits MemorySearchRequest |
| 2.2 | LongTermMemorySearchProcessor       | Searches LTM, emits MemoryEvent |
| 2.3 | FindMatchingConceptProcessor        | Assumes need to find concepts due to StuckThought, finds one or more in WM, so stops |
| 2.4 | (...)                               | What selects one of the concepts to try against? First cut: for now just pick single greedy option, in both ConceptInferenceProcessor and GapFillingProcessor. |
| 2.5 | ConceptInferenceProcessor           | Attempts to infer an identification of concept for '?' based on matching against concepts in WM. Emits a Percept if it discovers something better than what's already present. Emit new Percept theorising that '?' is a number. |
| 2.6 | GapFillingProcessor                 | Attempts to fill gap in partially parsed expression using concept/concepts available in WM, including any inferred concepts if present. Emit new Equation Percept, with '?' tagged as a number. |
| 2.7 | EquationEvaluationProcessor         | Needs to kick in a try again against new equation percept. Will fail once again. |
| 3.0 | (interceptor)                       | StuckThoughtEvent present |
| 3... | (...)                              | Now start employing strategies to guess at number value of '?' |

| x.x | FindMatchingConceptProcessor        | Last found concept(s) not good enough, tries again |


For attempt tracking, when first emiting StuckThoughtEvent, I think a processor needs to do some work before it is emitted:
* Currently adds top-most event to Event.references(), but there's probably no point specifically in tracking that one.
* Need to track the end of the chain at the time of stuck thought - so needs to navigate to end of chain, and reference that event.
* If it tracks anything else too, it would be about making an attempt to identify the event that best describes the current underlying request/problem that is stuck.

_(Added 2019-10-27. Labels: work-in-progress)_