# Install PredictionScan

Endpoint: `https://mcp.predictionscan.org/mcp`
Transport: Streamable HTTP. No API key or PredictionScan account required.

## Grok

Open https://grok.com/connectors, choose New Connector → Custom, enter name **PredictionScan** and the endpoint above, then Add Connector.

Tested November 1, 2026: Grok invoked the connector, returned market odds, weekly probability change and outcome-level flow, and rendered an interactive chart. This is custom installation; marketplace publication is separate.

## Perplexity

Open https://www.perplexity.ai/computer/plugins. Choose Add custom → Import plugin from GitHub and enter https://github.com/JordanKarst/predictionscan-mcp. Check that PredictionScan shows Installed and its connector shows Connected. In a new prompt, type `@predictionscan`, select the connector, and ask the sample below.

Tested November 1, 2026 on the available account: import, connection, market search and price history succeeded. Account and administrator availability may vary. This creates a personal installation, not a public Perplexity marketplace listing.

## Cursor

Merge this entry into your existing `.cursor/mcp.json` (preserve other servers):

```json
{
  "mcpServers": {
    "predictionscan": {"url": "https://mcp.predictionscan.org/mcp"}
  }
}
```

Alternatively import the Agent Plugins package where supported. Cursor-specific end-to-end testing remains pending.

## Other remote MCP clients

Add the endpoint using Streamable HTTP with no authentication. Eleven tools provide structured data and a plain-text fallback; interactive cards depend on host support. Registry identifier: `io.github.JordanKarst/predictionscan`, version `1.1.0`.

## Try it

“Use PredictionScan to find the December 2026 Fed decision market. Show the leading outcome, current probability and one-week change in percentage points. Include the returned analytics link and source.”

Then: “Show the last 24 hours of buy/sell/net flow for that outcome, with the actual coverage metadata.”

Prices change; do not treat sample values as expected constants. Market/trader links route through PredictionScan to PolymarketScan analytics. News links open the publisher. This integration reads public data and cannot trade or move funds.

## Remove

Disconnect/remove PredictionScan in the host’s plugin or connector settings. For Cursor, remove only this server entry from your configuration.
