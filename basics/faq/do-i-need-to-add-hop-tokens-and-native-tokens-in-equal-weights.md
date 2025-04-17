# Do I need to add Hop tokens and native tokens in equal weights?

No. It's perfectly fine to only provide one of the two tokens into the pool. You will still receive the same LP tokens as if you added two tokens.\
\
However, if you do decide to add two tokens you will notice that the interface might ask you to provide them in unequal ratios. Unlike AMM’s that use the [constant product formula](https://cryptotesters.com/blog/what-is-uniswap) (like Uniswap V2 or Sushiswap) liquidity is not added in equal weights with Hop. It can happen for example, that the Hop Pool interface asks you to put 7500 hUSDC and 10,000 USDC to become a liquidity provider.\
\
\
![Screenshot\_2021-07-30\_at\_17.00.03.png](https://help.hop.exchange/hc/article_attachments/4406102389645/Screenshot_2021-07-30_at_17.00.03.png)



This might be confusing to you because in a traditional AMM this would imply that hUSDC trades at a premium. However, when you actually try to **swap** hUSDC for USDC to arbitrage this seemingly skewed rate, the rate is actually close to 1.

This is caused by the stableswap pricing formula that the Hop AMM’s use but rest assured, you shouldn't face any impermanent loss. Even if you withdraw the tokens at a different ratio than when you deposited, you will still hold the same **dollar value** since 1hUSDC = 1 USDC ([how does hUSDC hold its peg?](https://help.hop.exchange/hc/en-us/articles/4406108935693)).\
\
So even if you deposit 7,500 hUSDC and 10,000 USDC and after one month you withdraw 9000 USDC and 8500 hUSDC (ignoring trading fees) you hold the same dollar value!
