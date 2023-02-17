# Roadmap

Per [HIP-14](https://forum.hop.exchange/t/rfc-protocol-fees-and-a-commitment-to-public-goods-funding/566), the DAO has decided to make the development of a V2 Core Messenger its priority for 2023. The V1 Asset Bridge has proven Hop's multichain infrastructure. This next phase opens it up for a whole ecosystem of applications ecosystem to be built on top.

### What is the Core Messenger?

The Hop Core Messenger is a simple, trustless messaging protocol that can be used to build powerful cross-chain applications.

How it works

* The Core Messenger uses a hub-and-spoke model
* Messages are aggregated into bundles
* The bundle is hashed and sent to the destination
* Native bridges with Ethereum are used to pass the bundle hash
* At the destination, messages in the bundle can be unpacked and executed

Because the native bridges can sometimes be slow, the Hop Core Messenger is best used for messages that require trustlessness and high-security but are not time sensitive (e.g. value settlement, dispute resolution, DAO governance, etc.).

Faster messaging models such as collateralized messaging and optimistic messaging (as seen in Hop V1) can be easily implemented on top of the Core Messenger for application-specific or generalized use cases.

### What can be built on top of the V2?

The Hop Roadmap foresees a myriad of modules to be built on top of this simple & trustless Messenger.

Modules will enable cross-chain functionality such as:

* Messaging
* Token transfers
* NFT transfers
* Omnichain tokens
* And many more custom use cases ✨

Among other things, the V2 will introduce much larger economies of scale as the amount of messages that can be added into Bundles increases the more applications develop on top of it. This will decrease costs and improve the capital efficiency of the asset bridge which is still the bread and butter vertical for Hop.

