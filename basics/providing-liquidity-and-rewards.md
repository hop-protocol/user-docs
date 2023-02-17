# Providing Liquidity & Rewards

In this section, we describe how you can begin providing liquidity in Hop and earn liquidity mining rewards. As mentioned, Hop has AMM's on each chain it supports. These AMM's effectively create markets between the canonical wrapped assets of the native bridges (e.g $USDC on Optimism) and between the Hop bridge tokens with the shortened challenge times (e.g $hUSDC on Optimism).\
\
When an individual provides liquidity to a pool, the individual receives an LP token which represents their individual share of the pool. This share becomes more valuable over time as it accrues fees generated from transfers.\
\
For example, imagine you provide 1 ETH into the $ETH pool on Arbitrum and receive 0.98 HOP-ETH-LP tokens. 1 year later you withdraw your liquidity from the pool (by burning the 0.98 HOP-ETH-LP tokens) and you receive 1.1 $ETH back. This means you will have earned 10%.

## How to Provide Liquidity (Step by Step)

First, you need to of course make sure you have assets on the network you want to provide liquidity on. As an example, if you want to provide liquidity in the $ETH pool on Arbitrum you will need to send $ETH to Arbitrum via Hop or alternatively through the [native Arbitrum bridge ](https://bridge.arbitrum.io/)(takes same time but Hop is often cheaper).&#x20;

### Step 1: Choose your Pool

Choose a pool based on the highest yield or the asset& network of your choice. Once you've decided you need to click on "Add liquidity" in the row of choice.

<figure><img src="../.gitbook/assets/Screenshot 2022-11-30 at 16.44.48.png" alt=""><figcaption></figcaption></figure>

### Step 2: Choose Amount

Clicking "Add liquidity" will lead you to the specific pool page of your choice. You'll see the 24hr volume, TVL as well as its APR.\
\
_In some cases you will need to_ [_wrap_](https://academy.binance.com/en/articles/what-is-wrapped-ether-weth-and-how-to-wrap-it?ref=AZTKZ9XS\&utm\_source=BinanceTwitter\&utm\_medium=GlobalSocial\&utm\_campaign=GlobalSocial) _your $ETH (same for $MATIC) to turn it into an ERC-20 token before depositing it into the pool. You will see a little prompt "Click here to Wrap or Unwrap" to do so._

You will see for each pool there's always two input fields. One for the "canonical" asset (e.g $ETH) and one for the Hop bridge token (e.g $hETH).\
\
Enter the amount you want to deposit into the input field of each token. You can provide single-sided (i.e only one asset) in which case you leave the other input field empty or provide both tokens in the ratio you like.

<figure><img src="../.gitbook/assets/Screenshot 2022-11-30 at 18.54.00.png" alt=""><figcaption></figcaption></figure>

### Step 3: Approve & Deposit

To start depositing your token(s), click the "Preview" button. A modal will appear showing you an overview of your transaction one last time before you actually deposit. If everything looks good you can hit the "Deposit & Stake" button. \
\
_If you don't wish to stake your LP tokens and earn $HOP liquidity mining rewards you can click the grey "Deposit" button just below. This will simply deposit your tokens but not stake the LP tokens._

<figure><img src="../.gitbook/assets/Screenshot 2022-11-30 at 19.44.42.png" alt=""><figcaption></figcaption></figure>

Assuming you have chosen to "Deposit & Stake" a wizard will walk you through all the necessary transactions and steps to stake your LP tokens. This will involve Approvals, Deposits and Stake transactions so expect to sign several transactions in your wallet. The good thing is, this happens on Layer-2 so the transactions are cheap and fast.

<figure><img src="../.gitbook/assets/Screenshot 2022-11-30 at 19.45.03.png" alt=""><figcaption></figcaption></figure>

\
\
Congrats you are now a liquidity provider in a Hop AMM and earning bridge fees + $HOP rewards  🥳
