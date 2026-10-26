# 4dlabs Daily Check-in

A Windows desktop app for running daily check-in transactions on BNB Smart Chain.

## Run the EXE

1. Download `4dlabsDailyCheckin.exe` from the project's GitHub Releases page (or download the EXE provided by the project owner).
2. Save it to a folder on your Windows PC.
3. Double-click `4dlabsDailyCheckin.exe` to launch the app.
4. On first launch, the app may create a `key.env` template in its working folder.
5. Add your own wallet private key or mnemonic phrase to `key.env`, one wallet per line, if you choose to use wallet-based check-ins.
6. Open the app, check the RPC URL, location, gas limit, and chain ID, then click **Save Settings**.
7. Click **START** to submit check-in transactions. Watch the Activity Log for transaction hashes, confirmations, and errors.

## Do I need to install Python?

No. The packaged one-file Windows executable includes Python and its bundled Python dependencies. You need a compatible Windows PC and an internet connection. You do not need to install Python, pip, or PyInstaller.

## Important wallet safety

- Never share your populated `key.env` file or publish it to GitHub.
- Never enter a wallet private key or recovery phrase into a build you do not trust.
- Use a dedicated wallet with only the funds needed for transaction fees.
- Blockchain transactions can be irreversible and may cost gas.
- Verify the network, RPC endpoint, contract address, and transaction details before clicking **START**.

## Troubleshooting

- **The app does not open:** Download the EXE only from a source you trust. Windows security software may warn about unsigned executables. Do not bypass warnings unless you have verified the file and publisher.
- **No valid keys found:** Check that `key.env` exists and contains valid wallet entries in the expected format.
- **Cannot connect to RPC:** Check your internet connection and the RPC URL.
- **Insufficient funds for gas:** The wallet needs enough native BNB to pay the transaction fee on BNB Smart Chain.
- **Transactions fail:** Verify the chain ID, contract address, contract availability, and configured gas limit.

## Configuration

The app defaults to BNB Smart Chain mainnet (chain ID `56`). Review all settings before running transactions. The app saves its settings to `config.json` when **Save Settings** is used.

## Disclaimer

Use at your own risk. You are responsible for protecting your wallet credentials and checking each transaction's network, destination contract, and cost.
