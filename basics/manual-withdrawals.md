# Manual Withdrawals

As a trustless bridge, Hop allows users to force exit their tokens in the rare event where Bonders (market makers) don’t bond a user’s transfer fast enough.\
\
This can happen because:\
\
1\) A Bonder fee was set too low (e.g if sent via a third-party app which miscalculates the Bonder fee)\
\
2\) Bonder is offline or misses on-chain events ( e.g because of RPC node issues)\
\
3\) Bonder is out of liquidity to bond Transfers or Transfer Roots.\
\
When this happens Hop offers users a fallback option to withdraw their tokens manually at the destination chain **albeit not as fast as it would arrive in a normal transfer** involving a fully functioning Bonder.\
\
In order to withdraw, the Transfer Root bundle containing the proof of your transaction must be propagated to the destination, and this **could take a few hours or days** depending on the asset and route, so withdrawing **immediately after sending won't work**.\
\
**Step 1: Paste your transaction hash**\
Go to the [withdraw ](https://app.hop.exchange/#/withdraw?token=ETH)[page UI](https://app.hop.exchange/#/withdraw?token=ETH) and paste the transaction hash of your transfer on the origin chain into the TransferID field.

![manual\_withdraw\_1.png](https://help.hop.exchange/hc/article\_attachments/7449225280781/manual\_withdraw\_1.png)

**Step 2: Withdraw your transfer**

If the Transfer Root containing your transaction has reached the destination chain you will see a pop-up. Click the “withdraw” button and confirm the transaction in your wallet.\
![manual\_withdraw\_2.png](https://help.hop.exchange/hc/article\_attachments/7449268621325/manual\_withdraw\_2.png)

**Step 3: Swap your hTokens for native tokens**

Upon showing your valid transfer proof the Hop bridge will mint hTokens for you (e.g hUSDC or hETH). So if you want native $USDC or $ETH you’ll need to manually convert your hTokens in the Hop AMM.\
\
Head to the “Convert” section in the Hop app, select the network and asset and choose the “via AMM” option to do the swap from hTokens into native tokens.\
\
NOTE: this final swap is only necessary if you sent to a Layer-2 network. If you sent to Ethereum you will **directly** receive native tokens, so no swap needed.\
![Screenshot\_2022-07-05\_at\_22.14.23.png](https://help.hop.exchange/hc/article\_attachments/7449261671437/Screenshot\_2022-07-05\_at\_22.14.23.png)\
\
