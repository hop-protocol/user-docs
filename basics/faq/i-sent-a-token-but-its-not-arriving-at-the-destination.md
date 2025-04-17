# I sent a token but it's not arriving at the destination

A normal L1 <> L2 transfer takes up to 15 minutes and a L2 <> L2 transfer up to 5 minutes (see [Hop transfer times](https://help.hop.exchange/hc/en-us/articles/4406099772045-How-long-does-a-Hop-transfer-take-)).\
\
In rare circumstances it can happen that the user receives **hTokens** instead of **native tokens** (e.g hUSDC instead of USDC) at the destination. This happens because the "swap" times out after a set deadline, meaning the Hop token doesn't get converted in the AMM of the destination chain. In these instances the user needs to convert their Hop tokens manually in the "Convert" tab to get the native token.\
\
Even more rarely, it can happen that there's no Bonder to "bond" your transfer and front the liquidity on the destination chain. This can can happen either because the Bonder is out of collateral (in which case you have to wait) or because of issues in the Bonder node infrastructure.\
\
If there is no Bonder liquidity at the destination chain there should be a warning in the Hop UI to let you know of the situation.\
\
If you still somehow send tokens while there is no Bonder liquidity your transaction will be pending until there is **new Bonder liquidity**.\
\
![Screenshot\_2021-09-20\_at\_14.52.35.png](https://help.hop.exchange/hc/article_attachments/4409642810893/Screenshot_2021-09-20_at_14.52.35.png)

\
