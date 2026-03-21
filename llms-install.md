# Installing Chainflip Broker as a Service MCP Server

This is a remote MCP server. No local installation, build steps, or API keys are required.

## MCP Configuration

Add the following to your MCP settings:

```json
{
  "mcpServers": {
    "chainflip-baas": {
      "type": "url",
      "url": "https://chainflip-broker.io/mcp"
    }
  }
}
```

## Transport

- **Type**: Streamable HTTP
- **URL**: `https://chainflip-broker.io/mcp`
- **Authentication**: None required

## Verification

After connecting, call the `list_assets` tool to verify the server is working. It should return a list of supported cryptocurrency assets with tickers, networks, and current USD prices.
