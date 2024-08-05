!!! tip "Support Hummingbot"
    Hummingbot Foundation has a fee share partnership with Tegro. When you use our software to trade on Tegro, a custom API header tells Tegro that the trade was executed using Hummingbot, so they share a portion of your fees with us, at no cost to you. To support us, create an account using our [Tegro referral link](https://www.tegro.com/en/register?ref=FQQNNGCD) or [Tegro Futures referral link](https://www.tegro.com/en/futures/ref?code=hummingbot) and enter that account's API keys into Hummingbot and run bots! Thanks for your support! 🙏

## 🛠 Connector Info

- **Exchange Type**: Decentralized Exchange (**DEX**)
- **Market Type**: Central Limit Order Book (**CLOB**)

| Component | Status | Connector Version | V2 Strategies | Notes | 
| --------- | ------ | ----------------- |  ------------ | ----- |
| [🔀 Spot Connector](#spot-connector) | ✅ | v2.1 | Yes | Supports `MARKET` order type
| [🔀 Perp Connector](#perp-connector) | Not available  |      |  | 
| [🕯 Spot Candles Feed](#spot-candles-feed) | Not available  | 
| [🕯 Perp Candles Feed](#perp-candles-feed) | Not available  |
| [📓 Connector Guide](/academy-content/using-tegro-with-hummingbot/) | ✅ | 

## ℹ️ Exchange Info

- **Website**: <https://www.tegro.com>


## 🔑 How to Connect

!!! tip
    See the [Tegro Connector Guide](/academy-content/using-tegro-with-hummingbot/) for details on create API keys on Tegro.

From inside the Hummingbot client, run `connect tegro`:

```
>>> connect tegro

Enter your Public Wallet Address >>>
Enter your Private Wallet Address>>>
Enter your preferred chain  >>>
```

If connection is successful:

```
You are now connected to tegro
```

## 🔀 Spot Connector
*Integration to spot markets API endpoints*

- **ID**: `tegro`
- **Connection Type**: WebSocket
- **API Docs**: <https://tegro-docs.github.io/apidocs/spot/en/>
- **[Github Folder](https://github.com/toraverse/hummingbot/tree/development)** 

### Order Types

This connector supports the following `OrderType` constants:

- `LIMIT`
- `LIMIT_MAKER`
- `MARKET`

### Paper Trading

Access the [Paper Trade](/global-configs/paper-trade/) version of this connector by running `connect tegro_paper_trade` instead of `connect tegro`.

If this is not available by default, you can configure Hummingbot to add this paper trade exchange. See [Adding Exchanges](/global-configs/paper-trade/#adding-exchanges) for more information.


### Order Types

This connector supports the following `OrderType` constants:

- `LIMIT`
- `LIMIT_MAKER`
- `MARKET`

### Position Modes

This connector supports the following position modes:

- One-way
- Hedge

### Paper Trading

This perp exchange offers a paper trading mode: <https://testnet.tegrofuture.com>

Afer you create an account and create the API keys, you can enter them by using the `connect tegro_perpetual_testnet` command within the Hummingbot client. Once connected, you should be able to use the testnet with the available perpetual strategies / scripts. 


- **ID**: `tegro`
- **Supported Intervals**: 1s | 1m | 3m | 5m | 15m | 30m | 1h | 2h | 4h | 6h | 8h | 12h | 1d | 3d | 1w | 1M
- **API Docs**: <https://tegro-docs.github.io/apidocs/futures/en/>
- **[Github Folder](https:/[/](https://tegro.readme.io/reference/introduction-1))** 
