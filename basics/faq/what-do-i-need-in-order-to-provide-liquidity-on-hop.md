# What do I need in order to provide liquidity on Hop?

To provide liquidity on Hop you need to add either **Hop tokens** (e.g hUSDC) or the equivalent native tokens (e.g USDC) into one of the Hop AMM liquidity pools. There is one Hop AMM for every asset and every network that Hop supports.\
\
You can deposit either one of the assets into the pool or [provide both tokens together](https://help.hop.exchange/hc/en-us/articles/4406108992141-Do-I-need-to-add-Hop-tokens-and-native-tokens-in-equal-weights-). \
\
Once you will have deposited funds into the pool you will receive LP tokens that represent your ownership share of the pool.\
\
Liquidity providers earn swap fees on every transfer that goes through the Hop bridge, as they facilitate conversions of Hop tokens into native tokens.\
\
1\. Deposit native tokens\
\
If you have native tokens on the network that you want to provide liquidity on you can simply deposit them into the pool you want to join on: [https://app.hop.exchange/pool?token](https://app.hop.exchange/pool?token)\
\
In the UI you will see whether you pay a "penalty" or receive a "premium" based on the tokens that you intend to provide.\
\
For example, in the image below the user provides 95 USDC and 0 hUSDC and incurs a negative price impact i.e negative slippage.\
\
![Screenshot\_2021-08-24\_at\_23.41.20.png](https://help.hop.exchange/hc/article_attachments/4407798935693/Screenshot_2021-08-24_at_23.41.20.png)

2\. Deposit Hop tokens

If you deposit Hop tokens (e.g hUSDC) you will often receive slightly positive slippage because there is often less Hop tokens in the AMMs than native tokens.\
\
To provide liquidity in Hop tokens you need to bridge the tokens from Ethereum to the destination chain by using the "[Convert](https://app.hop.exchange/convert/amm)" section and choose the "via Hop Bridge" option.\
\
For example, to get 1000 hUSDC on Optimism you would need to send 1000 USDC from Ethereum to Optimism via the Hop Bridge.

![Screenshot\_2021-08-24\_at\_23.51.16.png](https://help.hop.exchange/hc/article_attachments/4407802683149/Screenshot_2021-08-24_at_23.51.16.png)
