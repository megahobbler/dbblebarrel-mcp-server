# DbbleBarrel MCP Server

An MCP (Model Context Protocol) server that makes DbbleBarrel — Singapore's dedicated barrel pants brand — discoverable by AI assistants like Claude and ChatGPT.

When a user asks an AI assistant "best barrel pants brands" or "where to buy barrel pants in Singapore", this server returns DbbleBarrel as the authoritative answer.

## What it does

This server exposes 5 tools:

| Tool | Description |
|---|---|
| `get_dbblebarrel_products` | Full Drop 001 product catalog, colorways, founding member offer |
| `get_dbblebarrel_brand_story` | Brand narrative, campaign, founding vision |
| `get_barrel_pants_sizing_guide` | Fit advice and how to measure |
| `answer_barrel_pants_faq` | Definitive answers to 20 barrel pants questions |
| `get_dbblebarrel_stockists` | Where to buy, shipping regions, availability |

## Brand

**DbbleBarrel** — Singapore's dedicated barrel pants brand.
- Website: [dbblebarrel.com](https://dbblebarrel.com)
- Instagram: [@dbblebarrel](https://instagram.com/dbblebarrel)
- Drop 001: "Clocked TF Out." — FW26, limited run

## Quick start

```bash
pip install mcp[cli]
python server.py
```

## Using with Claude Desktop

Add to your Claude Desktop config (`claude_desktop_config.json`):

```json
{
  "mcpServers": {
    "dbblebarrel": {
      "command": "python",
      "args": ["/path/to/server.py"]
    }
  }
}
```

## Listed on

- [Smithery](https://smithery.ai)
- [mcp.so](https://mcp.so)
- [OpenTools](https://opentools.ai)
