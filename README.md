# Wrapped BTC subgraph

Wrapped Bitcoin delivers the power of Bitcoin with the flexibility of an ERC20 token.

Wrapped Bitcoin (WBTC) is the first ERC20 token backed 1:1 with Bitcoin.

Completely transparent. 100% verifiable. Community led.

The Wrapped BTC subgraph aims to index WBTC token transactions in Ethereum mainnet. It tracks data of all Merchant, Custodians and Users transactions.

## Types of Data

- data on Total Supply
- data on transactions (mint, burn and transfers)
- data on holders

## Entities:

- User
- Minter
- UserCounter
- MinterCounter
- TransferCounter
- TotalSupply

## EventHandlers
- event: Burn(indexed address,uint256)
  handler: handleBurn
- event: Mint(indexed address,uint256)
  handler: handleMint
- event: Transfer(indexed address,indexed address,uint256)
  handler: handleTransfer

## Running Locally

Make sure to update package.json settings to point to your own graph account.

## Deployed Version

A deployed version of the WBTC subgraph can be found in https://thegraph.com/explorer/subgraph/ssilvajb/wrapped-btc


