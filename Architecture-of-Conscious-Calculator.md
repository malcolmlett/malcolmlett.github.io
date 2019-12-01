The following diagram describes the high-level architecture of Conscious Calculator.

![Component and data flow diagram of conscious calculator](files/Component-and-data-flow-diagram-of-conscious-calculator-v1.png)

It contains the following major components:

|Component|Description|
|----|----|
|Attention Attenuator|Controls which input or processor output is selected for action and writing into Working Memory.|
|Working Memory|In human experiments this holds about 7 items for about 1 minute.|
|Short Term Memory|Records most recent events in chronological order. Acts like a swap-space to free up room in Working Memory.|
|Long Term Memory|Records significant events and learned concepts.|
|Conscious Feedback|Summarises the current state of working memory and feeds it back into the system as an input sense.|
|Interceptors|Slightly stateful event detectors and pre-processors of input senses.|
|Processors|Each processor is specialised to a particular recognition, prediction, or mental task. Don't have any of their own state.|