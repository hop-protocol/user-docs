# What happens if The Bonder bonds fraudulent transactions?

If the bonder attests to an invalid transfer root either maliciously or because of buggy software, anyone can challenge it. Imagine for example, The Bonder produces an invalid transfer root sending (minting) themselves 10,000 hUSDC on a different network. If this goes undetected the market would be flooded with fake (un-backed) hUSDC causing LP's a loss. \
\
However, the Hop protocol provides economic incentives for challenging a fraudulent transaction. The Bonder has to lock up 110% of the total value of the transfer root they bond as collateral -- in the event where a fraudulent transaction is detected 10% go to the challenger receives and the value of the fraudulent transaction is covered by The Bonder's stake. \
\
The challenge logic lives [here](https://github.com/hop-protocol/contracts/blob/master/contracts/bridges/L1_Bridge.sol#L268) and there's an open-source [Challenge Watcher](https://github.com/hop-protocol/hop/blob/develop/packages/hop-node/src/watchers/ChallengeWatcher.ts) that anyone can run.\
In the very near future, we are going to set up a notification system to Tweet if a bonder is fraudulent so that _anyone_ can see and challenge a transfer root.
