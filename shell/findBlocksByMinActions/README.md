Usage:

`./findBlocksByMinActions endEpoch epochCount minActions`

Description:

Searches all blocks for all epochs from endEpoch down to epochCount epochs in the past, and prints those blcoks that included at least minActions actions. This is useful to spot blocks with many actions included and correlate with effects on the network.

Example:

Extracts all blocks from epoch 16284 to 16285 that included at least 6 actions. 

```
./findBlocksByMinActions 16285 2 3
I'm looking for any block in epochs [16284..16285] with at least 3 actions included...

epoch, epoch block, chain block, num actions
16284, 404, 9907964, 3
16284, 594, 9908154, 3
16284, 603, 9908163, 3
16284, 604, 9908164, 3
16284, 605, 9908165, 3
16284, 606, 9908166, 4
16285, 36, 9908316, 3
16285, 38, 9908318, 3
16285, 57, 9908337, 4
16285, 225, 9908505, 3
16285, 325, 9908605, 3
16285, 478, 9908758, 3
16285, 568, 9908848, 3
16285, 591, 9908871, 3
16285, 611, 9908891, 3
16285, 706, 9908986, 3
``` 

