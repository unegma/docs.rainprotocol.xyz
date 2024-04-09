---
sidebar_position: 2
title: Getting started
---

### Download the app

First, head to the [download page](./1-download.md) and get a copy of the app.

### Settings

When you open the app for the first time you won't see any orders or vaults. This is because there can be many Raindex orderbook contracts across many chains, so you'll need to set them up.

Head to the settings page (link in the sidebar of the app) and paste in the settings below.

These are example settings for Raindex contracts currently deployed, but new versions are being deployed often so head over to the [Rainlang Telegram](https://t.me/+w4mJbCT6IfI2YTU0) to keep up with updates.

```
networks: 
  polygon: 
    rpc: https://rpc.ankr.com/polygon 
    chain-id: 137 
    network-id: 137 
    currency: MATIC
  mainnet: 
    rpc: https://1rpc.io/eth 
    chain-id: 1 
    network-id: 1 
    currency: ETH
  arbitrum-one: 
    rpc: https://1rpc.io/arb 
    chain-id: 42161 
    network-id: 42161 
    currency: ETH
  flare:
    rpc: https://rpc.ankr.com/flare 
    chain-id: 14
    network-id: 14
    currency: FLR
  bsc: 
    rpc: https://1rpc.io/bnb 
    chain-id: 56 
    network-id: 56 
    currency: BNB
  
subgraphs:
  polygon: https://api.thegraph.com/subgraphs/name/h20liquidity/polygon-0xc95a5f8e
  mainnet: https://api.thegraph.com/subgraphs/name/h20liquidity/ethereum-0xf1224a48
  arbitrum-one: https://api.thegraph.com/subgraphs/name/h20liquidity/arbitrum-0x90caf23e
  flare: https://subgraphs.h20liquidity.tech/subgraphs/name/flare-0xb06202aA
  bsc: https://api.thegraph.com/subgraphs/name/h20liquidity/binance-0xb1d6d105

orderbooks:
  polygon:
    address: 0xc95A5f8eFe14d7a20BD2E5BAFEC4E71f8Ce0B9A6
    network: polygon
    subgraph: polygon
  mainnet:
    address: 0xf1224A483ad7F1E9aA46A8CE41229F32d7549A74
    network: mainnet
    subgraph: mainnet
  arbitrum-one:
    address: 0x90CAF23eA7E507BB722647B0674e50D8d6468234
    network: arbitrum-one
    subgraph: arbitrum-one
  flare:
    address: 0xb06202aA3Fe7d85171fB7aA5f17011d17E63f382
    network: flare
    subgraph: flare
  bsc:
    address: 0xf1224A483ad7F1E9aA46A8CE41229F32d7549A74
    network: bsc
    subgraph: bsc

deployers:
  polygon:
    address: 0xF77b3c3f61af5a3cE7f7CE3cfFc117491104432E
    network: polygon
  mainnet:
    address: 0x4D69ec4d0112E42c385B5cCb6897cCdfeAfC3136
    network: mainnet
  arbitrum-one:
    address: 0x2AeE87D75CD000583DAEC7A28db103B1c0c18b76
    network: arbitrum-one
  flare:
    address: 0x550878091b2B1506069F61ae59e3A5484Bca9166
    network: flare
  bsc:
    address: 0x1eFd85E6C384fAD9B80C6D508E9098Eb91C4eD30
    network: bsc
```

### Deploying your first order

You should now see orders and vaults across multiple networks on the Orders and Vaults pages.

Try deploying your first order by following one of [the examples](./example-strats/1-examples.md).