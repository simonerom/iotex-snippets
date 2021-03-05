Usage:
`./findBlocksByMinActions endEpoch epochCount minActions`

Description:
Searches all blocks for all epochs from endEpoch down to epochCount epochs in the past, and prints those blcoks that included at least minActions actions. This is useful to spot blocks with many actions included and correlate with effects on the network.

Example:

`./findBlocksByMinActions 16285 10 10` 

tells extracts all blocks from epoch 16276 to 16285 that included at least 10 actions. 
