# Harbor Testnet with One Chain (Ethereun) and Two Off-Chain Actors (Postgres and Liquidation bot)

This is to demosntrate configuring, building and running a sample Testnet with one chain (Ethereum) and two actors (Postgres and Liquidation bot). Clone this repo and follow along.

## Copy credentials

### User Key
On your home page, you should be able to copy your User Key which is found on the top right of the page.

### Project Key
In your projects page, each project has a Project Key that you can copy.

## Configure your credentials

Run the command:

```bash
harbor configure keys
```

This will ask you to add in your credentials, which includes your User Key and Project Key. Find them in the app and paste them here.

## Start Testnet

To run the Testnet, execute the following command in the same directory as this project:

```bash
harbor apply <testnet-name>
```

You should see this:

```bash
Checking ~/.harbor for your apiKey
Validating testnet name...
Configuring chain...
Configuring off-chain actor liquidation-bot-1
Configuring off-chain actor postgres
```

At the end of the logs, you should see your chain and off-chain actors with endpoints:

```bash
These are your running processes and their ports
ethereum
3.91.12.13:4000

postgres
3.91.12.13:5432

liquidationBot
3.91.12.13:3000
```

You can now interact with them using the endpoints.
