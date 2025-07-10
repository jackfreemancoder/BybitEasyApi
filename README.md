
# Bybit Easy API

Bybit Easy API is a simple and efficient .NET client library for interacting with the Bybit cryptocurrency exchange API. It provides easy-to-use methods to access Bybit’s public and private endpoints, allowing developers to integrate Bybit trading functionality into their applications seamlessly.

## Features
- Access public market data endpoints
- Place and manage orders
- Retrieve account information and balances
- Handle real-time WebSocket data streams
- Easy authentication with API keys
- Asynchronous programming support for high performance

## Installation

You can install the package via NuGet Package Manager:

```bash
Install-Package Bybit
```

Or via .NET CLI:

```bash
dotnet add package Bybit
```

## Usage
REST Endpoints
```csharp
// Get the ETH/USDT ticker via rest request
var restClient = new BybitRestClient();
var tickerResult = await restClient.V5Api.ExchangeData.GetSpotTickersAsync("ETHUSDT");
var lastPrice = tickerResult.Data.List.First().LastPrice;
```
Websocket streams
```
var socketClient = new BybitSocketClient();
var tickerSubscriptionResult = socketClient.V5SpotApi.SubscribeToTickerUpdatesAsync("ETHUSDT", (update) =>
{
	var lastPrice = update.Data.LastPrice;
});
```
## Documentation

Detailed documentation is available on the [GitHub repository](https://github.com/jackfreemancoder/BybitEasyApi).

## Contributing

Contributions are welcome! Please open issues or submit pull requests via the GitHub repository.

## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/jackfreemancoder/BybitEasyApi/blob/main/LICENSE) file for details.

---

*By Jack Freeman*

