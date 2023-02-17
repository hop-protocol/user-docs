# How long does a transfer take?

It depends which network you are sending to and from. As a general rule of thumb, L1 to L2 transfers take the same amount of time than sending via the native bridge. For example, depositing from Ethereum to Polygon takes approximately 22 minutes via the Polygon bridge and the same amount of time with the Hop bridge. This is because Hop **itself** uses the native bridges for L1 -> L2 deposits.\
\
The advantages with Hop come about when you transfer **the other way around** from L2 to L1 or from one L2 to another L2.\
\
Here, the rule of thumb is that an exit will take as many blocks to be considered final (safe from [reorgs](https://www.paradigm.xyz/2021/07/ethereum-reorgs-after-the-merge/)) on the sending chain.\
\
_FYI: Hop has a_ [_multichain block explorer_](https://explorer.hop.exchange/) _which allows you to track the status of your transaction as well as all your past transactions._

### L2 to Any

* Optimism: trusted sequencer -> <5 minutes
* Arbitrum: trusted sequencer -> <5 minutes
* Nova: trusted sequencer -> <5 minutes
* Polygon: 256 blocks -> <20 minutes
* Gnosis: 12 blocks -> <5 minutes

### Ethereum to Any

* Optimism: \~10 min
* Arbitrum: <20 min (Finality based)
* Polygon: <30 min (Finality based)
* Gnosis: \~5 min
