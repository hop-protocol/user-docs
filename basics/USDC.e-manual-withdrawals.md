# USDC.e Manual Withdrawals

As the Hop USDC bridge was upgraded to utilize Circle's CCTP, leading to the deprecation of the USDC bonder, transfers involving USDC.e now require manual withdrawal.\
\
Hop enables you to withdraw hUSDC.e from the pool and transfer it to L1 at a 1:1 ratio. However, transferring hUSDC.e to L1 requires completing the full exit process, which takes at least 7 days after the root commit before the withdrawal can be finalized. To proceed, follow the steps below:\
\
**Step 1: Initiate the bridge to L1**\
Go to the [convert page UI](https://app.hop.exchange/#/convert/hop), select origin chain and make sure convert method is set to "via Hop Bridge".\
Initiate the transfer by clicking the "Convert" button.
![image](https://github.com/user-attachments/assets/4b62d9b4-0c72-4ec5-bccd-622ab8c14636)


**Step 2: Submit "Commit transfers" transaction**\
Visit the [relay UI](https://app.hop.exchange/#/relay) and paste the transaction hash of your transfer on the origin chain into the TransferID field.\
This will initiate the "Commit transfers" transaction.
![image](https://github.com/user-attachments/assets/6c4864c1-3e08-43ac-8811-7be57a85937c)

**Step 3: Submit "Prove Withdrawal" transaction**\
On the same [relay UI](https://app.hop.exchange/#/relay) page, initiate the "Prove Withdrawal" transaction on L1 by clicking the "Relay" button again.

Alternatively, you can complete this step using [superchainrelayer.xyz](https://superchainrelayer.xyz/) by pasting the transaction hash of the "Commit transfers" transaction you executed in Step 2 and clicking on "Prove tx".
**This will initiate the 7-day exit period.**
![image](https://github.com/user-attachments/assets/8686e83d-b811-4a43-aff0-c085142d6360)

**Step 4: Submit "Finalize Withdrawal" transaction**\
Visit the [relay UI](https://app.hop.exchange/#/relay) and paste the transaction hash of your transfer on the origin chain into the TransferID field.\
This will initiate the "Finalize Withdrawal" transaction.

Alternatively, you can complete this step using [superchainrelayer.xyz](https://superchainrelayer.xyz/) by pasting the transaction hash of the "Commit transfers" transaction you executed in Step 2 and clicking on "Finalize tx".
![image](https://github.com/user-attachments/assets/e3570586-7f5e-4a3c-a213-472129d8ca48)

**Step 5: Withdraw your transfer**\
Go to the [withdraw ](https://app.hop.exchange/#/withdraw?token=ETH)[page UI](https://app.hop.exchange/#/withdraw?token=ETH) and paste the transaction hash of your transfer on the origin chain into the TransferID field.\
Click the “withdraw” button and confirm the transaction in your wallet.
![image](https://github.com/user-attachments/assets/b90be264-ccd0-4070-ac35-9a26c2c5a649)
