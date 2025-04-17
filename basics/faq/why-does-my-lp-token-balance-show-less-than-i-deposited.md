# Why does my LP token balance show less than I deposited?

You deposited $20,000 and recieve 18,000 LP tokens. This is normal and not a reason for concern. The LP tokens reflect your relative ownership of the pool are not meant to reflect 1:1 the amount of tokens you deposited. The dollar value of your LP tokens changes constantly as the trading pool earns swap fees.

Say you provide liquidity to the pool and receive 1000 LP tokens in return, and let's assume that 1 LP token is worth 1$ at the time you deposit. From the moment you deposit the value of each LP token keeps increasing due to fees accumulated in the liquidity pool. One month later when you decide to withdraw your funds in the pool, you will send back your 1000 LP tokens and receive **more** than $1000 in the token you deposited. This is because the liquidity pool has earned trading fees during this 1 month period and so every single one of your 1000 LP tokens is now worth a little more than 1$.

**Advanced**

You can calculate yourself how much your LP tokens are worth at any point in time by checking the total number of LP tokens that exist for the pool.

1\) Go to the contract page of the LP token on a block explorer ( e.g[ LP token of USDC - hUSDC pool](https://polygonscan.com/token/0x9d373d22fd091d7f9a6649eb067557cc12fb1a0a)) and check the total supply of LP tokens in circulation

&#x20;

2\) Let this number be N (at the time of writing it's 4,378,343)

&#x20;

3\) Check how many USDC and hUSDC are in the liquidity pool on a block explorer (e.g[ hUSDC - USDC pool](https://polygonscan.com/address/0x5c32143c8b198f392d01f8446b754c181224ac26))

&#x20;

4\) Calculate your share of tokens in the pool based on your LP tokens

&#x20;

\=> Say the number of USDC tokens is U and the number of hUSDC tokens is H. If you own x LP tokens they then represent x/N \* U USDC tokens and x/N \*H hUSDC tokens.

**Example**:

Your LP tokens: 100

Total LP tokens: 4,378,343

USDC in pool: 2, 338,561

hUSDC in pool: 2,125,578

&#x20;

**Calculation:**

1\) 100/4,378,343 \* 2, 338,561 = 53.41 USDC

2\) 100/4,378,343 \* 2,125,578 = 48.54 hUSDC

&#x20;

So in this example your LP tokens are worth $102.
