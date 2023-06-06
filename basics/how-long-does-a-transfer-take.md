# How long does a transfer take?

It depends which network you are sending to and from. As a general rule of thumb, L1 to L2 transfers take the same amount of time than sending via the native bridge. For example, depositing from Ethereum to Polygon takes approximately 22 minutes via the Polygon bridge and the same amount of time with the Hop bridge. This is because Hop **itself** uses the native bridges for L1 -> L2 deposits.\
\
The advantages with Hop come about when you transfer **the other way around** from L2 to L1 or from one L2 to another L2.\
\
Here, the rule of thumb is that an exit will take as many blocks to be considered final (safe from [reorgs](https://www.paradigm.xyz/2021/07/ethereum-reorgs-after-the-merge/)) on the sending chain. Some chains determine finality based on L1 consensus. The time-to-finality for these chains is not constant, so the values below will be an average based on the `safe` status of a block that a transaction is included in.\
\
_FYI: Hop has a_ [_multichain block explorer_](https://explorer.hop.exchange/) _which allows you to track the status of your transaction as well as all your past transactions._

### L2 to Any

* Optimism: \~12 minutes (finality)
* Arbitrum: \~12 minutes (finality)
* Nova: \~12 minutes (finality)
* Polygon: \~22 minutes (512 blocks)
* Gnosis: \~2 minutes (finality)

### Ethereum to Any

* Optimism: \~3 minutes (optimistic finality)
* Arbitrum: \~10 minutes (finality)
* Polygon: \~25 min (finality)
* Gnosis: \~30 min (light client finality)
