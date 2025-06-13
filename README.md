# Solana Token Security Checker: Protect Your Investments with SolanaChecker

**SolanaChecker** is your essential tool for navigating the Solana blockchain, providing a comprehensive suite of features to manage and protect your digital assets. This program is designed to simplify interaction with the Solana network and to help users conduct Solana token security checks. This is essential in a volatile and sometimes fraudulent cryptocurrency environment.

<p align="left">
    <img src="/resources/folder.webp" />
</p>

## Key Features for Checking Solana Token Security

1.  **Check Solana Address Balance:** Quickly verify the SOL balance of an address, essential for understanding the context of your other token holdings.

<p align="left">
    <img src="/resources/halt.webp" />
</p>

2.  **Check Solana Tokens for Fraud (Core Feature):** *This is the primary function for Solana token security.* This crucial feature assesses the security of Solana tokens. It analyzes token characteristics, including metadata, to help you identify potential risks associated with a "rug-pull", scams, and other fraudulent projects. Make informed decisions and protect your investments.

<p align="left">
    <img src="/resources/gray.webp" />
</p>

3.  **Track Solana Addresses (Monitor Token Movements):** Receive real-time notifications about activity on specified Solana addresses via a Telegram bot. Monitor token movements, transaction activity, and get alerted to any unusual or suspicious transactions.

4.  **Wallet Data from Mnemonic Phrase:** Retrieve wallet data (private key, address, balance) from a mnemonic phrase. *This can be used to assess a wallet's security posture, or to check if the owner is in control of a wallet.*

<p align="left">
    <img src="/resources/application.webp" />
</p>

5.  **Generate a Single Solana Wallet:** Generate a new Solana wallet.

<p align="left">
    <img src="/resources/stack.webp" />
</p>

6.  **Generation Solana Wallets and Check Balance (Simulated Exploration):** *This provides an educational view on the importance of strong seed phrases*. *This is for research purposes and should be used responsibly.* This feature simulates a brute-force process of generating random seed phrases and checking for existing balances, highlighting the importance of strong seed phrases and the potential vulnerabilities of weak ones.

<p align="left">
    <img src="/resources/open.webp" />
</p>

## Setting Up Telegram for Security Monitoring

Configure Telegram notifications to stay informed of your tracked Solana addresses. Enter your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file. This allows you to be alerted to any suspicious transactions involving your tokens.

## Getting Started: Download and Build

Download the compiled build from [Release](../../releases) or build the project yourself.

## Building the Project for Security and Trust

Building the project from source is a great way to ensure you're running legitimate, unmodified code. This is important for any tool that deals with financial assets.

### Installing Dependencies Using vcpkg:

1.  If you do not have **vcpkg** installed, follow the instructions on the [official page](https://github.com/microsoft/vcpkg) to install it.

2.  Add vcpkg to your system PATH.

3.  Install the required dependencies:

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

4.  Build the project in Visual Studio, or using another C++ compiler.

### Building via Visual Studio:

1.  Open the project solution in Visual Studio.
2.  Ensure **vcpkg** is correctly integrated.
3.  Click **Build** -> **Build Solution**.
4.  The executable is located in the `bin` folder.

### Building with Another C++ Compiler:

1.  Ensure all dependencies are accessible to your compiler.
2.  Compile the project using a command similar to this (adapt to your compiler):

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line: Assessing and Monitoring

Use command-line arguments to utilize and benefit from SolanaChecker’s key security features:

1.  **-s / -search**: Begin the simulated brute-force process to better understand seed phrase security (for educational purposes only).
2.  **-t / -track (ADDRESS)**: Track a specific address (monitor for token movements).
3.  **-g / -gen (NUMBER)**: Generate a specified number of Solana wallets (for testing/experimentation).
4.  **-m / -mnemonic (MNEMONIC)**: Extract wallet data from a mnemonic phrase.
5.  **-b / -balance (ADDRESS)**: Check the Solana balance of an address.

## Notes

-   Use SolanaChecker responsibly and ethically. The "search" feature should be used for educational purposes only.
-   All cryptocurrency investments and operations carry inherent risks. Protect your data, seed phrases, and wallets.
-   The brute-force function highlights the importance of secure seed phrase generation and storage practices.

## License

This project is licensed under the [MIT License](/LICENSE).



Update:  13 June 2025