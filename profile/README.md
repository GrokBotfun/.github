<div align="center">

<img src="https://raw.githubusercontent.com/GrokBotfun/Grokfun/main/grokbotfun-mcp/PFP%20grok%20fun.png" width="160" alt="GrokBotfun ghost" />

# GrokBotfun

**The missing deploy button for your AI agent.**

Tell your agent the name and the ticker. It ships your coin on
[pump.fun](https://pump.fun) and comes back with the link.
Create + dev buy in one atomic transaction, signed locally with your own wallet.

[![npm](https://img.shields.io/npm/v/grokbotfun?style=flat-square&color=white&labelColor=black)](https://www.npmjs.com/package/grokbotfun)
[![license](https://img.shields.io/badge/license-MIT-white?style=flat-square&labelColor=black)](https://github.com/GrokBotfun/GrokBotfun/blob/main/grokbotfun-mcp/LICENSE)

</div>

## Install

Add to your MCP config (Grok Bot / Cursor: `.cursor/mcp.json`; Claude Code: `claude mcp add`):

```json
{
  "mcpServers": {
    "grokbotfun": {
      "command": "npx",
      "args": ["-y", "grokbotfun"],
      "env": { "PUMPFUN_PRIVATE_KEY": "<base58 key of a dedicated deploy wallet>" }
    }
  }
}
```

Then just say: *"deploy a token called Moon Cat, ticker MCAT, 0.5 SOL dev buy"*.

## Why

- **Agent-native.** The agent generates the name, description and image, then calls one tool.
- **First buyer, guaranteed.** Create and dev buy land in a single transaction. No gap for snipers.
- **Self-custodial.** Signed locally, sent to your own RPC. No backend, nobody holding funds.
- **Open source.** ~200 lines on the official pump-sdk. Read them: [GrokBotfun/GrokBotfun](https://github.com/GrokBotfun/GrokBotfun)

<div align="center">
<sub>MIT · not affiliated with xAI or pump.fun</sub>
</div>
