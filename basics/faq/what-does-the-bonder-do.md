# What does “The Bonder” do?

A Bonder must stake (lock-up) collateral to be used as credit for transfers in order to guarantee liquidity on the destination rollup. In other words they advance liquidity on the destination chain to make the transfer instant for the user as opposed to having to wait a couple of days if they were to use the native rollup bridges. In exchange, they take a small fee (0.02%).\
\
The Bonder’s stake is treated like credit. The **credit** is **subtracted** when individual transfers are **bonded** and **re-credited** when **transfers are settled**.\
\
Transfers are settled when the bonded transfer root is propagated from layer-2 to layer-1 after the rollup/sidechain challenge period.

\
