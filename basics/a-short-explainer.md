# A Short Explainer

Hop is a scalable rollup-to-rollup general token bridge. It allows users to send tokens from one rollup or sidechain to another almost immediately without having to wait for the networks challenge period.\
\
It works by involving market makers (referred to as Bonders) who front the liquidity at the destination chain in exchange for a small fee.\
\
This credit is extended by the Bonder in form of hTokens which are then swapped for their native token counterpart in an AMM on the destination chain.

The end result allows users to seamlessly transfer tokens from one network to the next.

The hTokens exist to allow the protocol to mint & burn tokens programatically to move them across chains more easily but also to shorten the native exit time of each scaling solution and allow Bonders to be more capital efficient. Bonders unlock their fronted capital every 24hrs.

### Hop is trustless

Users have on-chain guarantees that they will receive their funds even in the event where Bonders are offline. In the rare event where this happens, users have to wait until the on-chain proof is propagated to the destination chain to withdraw their tokens manually. In the worst case users will face a slow experience but their funds can't be taken by the Hop bridge.

### Liquidity is automatically rebalanced

By virtue of having AMM's on each chain, liquidity always flows to where its most needed. If a lot of user funds are bridged from say Optimism to Ethereum, arbitrageurs will be economically incentivized to bridge the other way to pocket a premium and thereby rebalance the pools.&#x20;

### Hop is powered by a set of Bonders

Bonders run local nodes to verify if the state transitions on the source chain are accurate and decide to "bond" the transfer by locking up 110% of the `TransferSum` as collateral. This allows them to mint hTokens at the destination chain which are sent to the user to provide instant liquidity. The Bonder unlocks the capital after a 24hr challenge period during which anyone can challenge the Bonder. If a challenge is successful the Bonder capital is slashed.\
\
For more info about Hop V1 please refer to our [whitepaper](https://hop.exchange/whitepaper.pdf).
