# What are the fees for transfering tokens with Hop?

There is no simple answer for this question as the overall cost of your transfer will depend on various factors.\
\
![Screenshot\_2021-09-20\_at\_13.35.26.png](https://help.hop.exchange/hc/article_attachments/4409648170893/Screenshot_2021-09-20_at_13.35.26.png)\
\
**1. AMM swap fees (0.04%)**\
\
When you transfer e.g USDC from Optimism to Arbitrum your USDC will be converted into hUSDC in the USDC AMM on Optimism costing **a 0.04% fee**.\
\
Then this hUSDC will be burned and a Bonder will bond your transfer by locking his collateral and mint you some new hUSDC on Arbitrum. \
\
This hUSDC will now be converted in the Arbitrum USDC AMM for canonical USDC costing **another 0.04%.** \
\
L2 <> L2 -> 0.08% swap fees (because two swaps)\
L2 -> L1 -> 0.04% (because only one swap)\
\
**2. Slippage (?%)**\
\
Depending on the liquidity in the AMM's the rate for conversions between hTokens and canonical tokens can fluctuate and eat into the cost of your transfer. With more liquidity in the Hop protocol and actors arbitraging the pools this should become less and less of a problem.\
\
**3. Bonder fee (0.06-0.25%)**\
\
The Bonder takes a fee for fronting the liquidity of your transfer at the destination chain and taking on risk.\
\
The fee varies per asset and per route based on the transaction volume and other factors due to economies of scale. If there is a lot of demand for an asset, Bonder fees can be lowered while still breaking even.\
\
\
**4. Destination chain tx fee (gas fees)**\
\
The funds need to be sent from the Bonder to your wallet and users need to pay for this gas cost.\
This gas cost is factored into the fee the user pays on the origin chain and displayed before sending.\
\
**5. Minimum fee ($1)**\
\
To prevent spamming there is a minimum fee of $1 per Hop transfer. I.e if the total fee paid by the user is < $1 it will be rounded up to $1.\
\
&#xNAN;_\* Overview of Bonder fees_\
\
![bonder\_fees.png](https://help.hop.exchange/hc/article_attachments/4416476354189/bonder_fees.png)\
\


\
