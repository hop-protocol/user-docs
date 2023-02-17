# What is special about Hop?

#### Intro to Bridges

Every bridge relies on a mechanism to transfer data across chains. In some way or another, it needs to be proven that a given transfer on a source chain is valid and that the bridge protocol can release tokens to the user on the destination chain. This is how the native settlement times can be bypassed and how assets can be transferred between L2's even though they are not directly connected.

Bridges differ in _how they transfer data between chains_ and this is what defines their security model for the most part.&#x20;

Most bridges rely on some **off-chain actors** like a multisig or oracle to certify that a transfer happened. This means there's an off-chain attack vector. Keys can be compromised. And this is not an abstract threat. Over [$3 billion of capital](https://assets.ctfassets.net/4rilomtvvae4/5DgOdTmxer4KBlLsOTXapd/b19f517260fa1f0d25c87b79fd88944c/2022\_Year\_in\_Review\_-\_Arcane\_Research.pdf) locked in bridges have been hacked in 2022 and the majority of these hacks were due to key compromises.

#### How Hop is Different

Hop has been built with maximal security in mind. There are no single point of failures or trusted off-chain actors. Instead the security is 100% rooted on-chain.

Hop compresses origin messages (i.e transfers) into Bundles and uses the native message bridges to transfer these Bundles between chains. This system is refered to as using a "Hub-and-Spoke" model where Ethereum is the main hub through which everything is routed and each scaling solution is a spoke. For example, to send data between Optimism and Arbitrum, Hop will send a Bundle down to Ethereum through the native Optimism bridge and then up to Arbitrum again using the native bridge. This means the **validity of a transfer can be proven on-chain**!

Now this way to transfer data is maximally secure but you might have noticed that it's also slower as it depends on the native message bridges' exit times (40 mins for Polygon PoS and Gnosis Chain and up to 7 days for ORU's).&#x20;

This is why the Bonders exist. They verify transactions off-chain and front the liquidity for the users on the destination chain. By doing so they take the liquidity lock-up upon them and have their liquidity unlocked once the on-chain proof (aka Bundle) arrives at the destination.

#### Why Security is Important

This security model gives Hop a competitive advantage. All else equal, bridges with weaker security model will need to pay higher interest rates to attract liquidity than trustless bridges. Over the long term, as the markets understanding of bridges matures, it is highly likely that trustless bridges will be able to offer lower bridging fees than centralized bridges.

The security of its Core Messenger will also be appreciated as Hop continues to venture into interoperability use cases beyond asset bridging such as: cross-chain governance, NFT bridging, omnichain tokens etc.
