# PredictionScan

Derived analytics for researching real-world events with prediction markets.

PredictionScan combines outcome-level buy/sell flow, historical probability changes, large-trade context, public trader research and market-matched news. Eleven read-only tools are available without an API key. Public market data originates from Polymarket; PredictionScan adds aggregation, filtering, ranking and news matching. Independent; not affiliated with or endorsed by Polymarket.

## Connect

MCP endpoint: `https://mcp.predictionscan.org/mcp`
Transport: Streamable HTTP. Authentication: none.

Install this Agent Plugins package in a compatible host, or add the URL as a custom remote MCP connector. Host plan and administrator restrictions may apply.

Try: “Find the December Fed decision market, show its odds and one-week probability change, then summarize buy/sell flow by outcome and relevant headlines.”

Tools: search_markets, get_market_odds, get_price_history, get_market_movers, get_trending_markets, get_whale_trades, get_market_flow, get_leaderboard, get_trader_profile, get_trader_positions, get_market_news.

Results include text and structured data. Compatible hosts can render MCP Apps cards. Market/trader links use PredictionScan’s existing routing to analytics pages on PolymarketScan. News links open their publishers. The plugin cannot trade, transfer funds or connect wallets. Market probabilities are crowd forecasts, not certainty or advice. Partial data and coverage limits must be retained when summarizing results.

Website: https://predictionscan.org/
Support: https://predictionscan.org/support
Privacy: https://predictionscan.org/privacy
Terms: https://predictionscan.org/terms

Operator: PM Data Services.

This portable distribution copy is separate from the already-approved OpenAI release and the existing Claude submission. Do not upload it over either existing release.
