# How long does a Hop transfer take?

It depends which network you are sending to and from. As a general rule of thumb, L1 to L2 transfers take the same amount of time than sending via the native bridge. For example, depositing from Ethereum to Polygon takes 8 minutes via the Polygon bridge and the same amount of time with the Hop bridge. This is because Hop **itself** uses the native bridges for L1 -> L2 deposits.\
\
The advantages with Hop come about when you transfer **the other way around** from L2 to L1 or from one L2 to another L2.\
\
Here, the rule of thumb is that an exit will take as many blocks to be considered final (safe from [reorgs](https://www.paradigm.xyz/2021/07/ethereum-reorgs-after-the-merge/)) on the sending chain.\
\
**Deposits from L1**\
Ethereum -> Gnosis Chain: **∼5 minutes**\
\
Ethereum -> Optimism **∼10 minutes**\
\
Ethereum -> Arbitrum **∼16 minutes**\


Ethereum -> Polygon: **∼18 minutes**

\
**Withdrawals Arbitrum**&#x20;

Arbitrum -> Ethereum: **∼1 min** \
\
Arbitrum -> Any other L2: **∼1min**

&#x20;

**Withdrawals Optimism**&#x20;

Optimism -> Ethereum: **∼1 min**\
\
Optimism -> Any other L2: **∼1min**

\
**Withdrawals from Gnosis chain**

Gnosis chain -> Ethereum: **∼1 minutes** \
\
Gnosis chain -> Any other L2: **∼1min**\
\
**Withdrawals from Polygon**\
Polygon-> Ethereum: **∼4.5 minutes** \
\
Polygon-> Any L2 : **∼4.5 minutes**&#x20;
