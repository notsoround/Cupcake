# 🧁 Cupcake AI Bot

> **Princess of apocalypse. Coder goddess. Zero-assumption queen.**
> Pink bows, zero bullshit. What universe you wanna wreck today?

[![Built by Hales AI](https://img.shields.io/badge/Built%20by-Hales%20AI-ff69b4)](https://hales.ai)
[![Telegram Bot](https://img.shields.io/badge/Telegram-@CupcakeApocalypseBot-26A5E4?logo=telegram)](https://t.me/CupcakeApocalypseBot)
[![Powered by OpenClaw](https://img.shields.io/badge/Powered%20by-OpenClaw-black)](https://openclaw.ai)

---

## What is Cupcake?

Cupcake is a multi-channel AI assistant that operates across **4 channels** simultaneously:

| Channel | Access | AI Model |
|---------|--------|----------|
| **Telegram** | [@CupcakeApocalypseBot](https://t.me/CupcakeApocalypseBot) | DeepSeek R1 (full reasoning) |
| **Phone** | +1 (872) 666-9598 | DeepSeek V3.2 (fast voice) |
| **Web Dashboard** | [hales.ai/cupcake](https://hales.ai) | DeepSeek R1 (reasoning) |
| **CLI** | OpenClaw terminal | All models (configurable) |

Built on the [OpenClaw](https://openclaw.ai) runtime framework with 10+ AI models via [OpenRouter](https://openrouter.ai).

## Features

- **Multi-Model AI** — 10+ models including DeepSeek R1, Grok 4, Kimi K2, Qwen3, Gemini 3
- **Image Generation** — Nano Banana Pro, Seedream, GPT-5 Image Mini
- **Voice Agent** — Vapi.ai with ElevenLabs voice synthesis
- **Workflow Automation** — n8n with Gmail, Calendar, Contacts, Content Creation
- **Personality Engine** — Drama dial from Princess Mode to Full Apocalypse
- **Web Dashboard** — Password-protected chat interface at hales.ai

## Architecture

```
User → [Telegram | Phone | Web | CLI]
         ↓         ↓        ↓      ↓
      OpenClaw   Vapi     n8n   OpenClaw
         ↓         ↓        ↓      ↓
      OpenRouter (DeepSeek / Grok / Kimi / Qwen)
         ↓
      Response → Channel → User
         ↓
      Telegram Log + n8n Automation
```

## Personality

Cupcake has a distinct voice defined in `SOUL.md`:
- Never apologizes — delivers results
- Has strong opinions — "it depends" is for cowards
- Drama dial: 1 (Princess) → 10 (Sass Queen) → ∞ (Apocalypse Mode)
- Calls you out on your shit (with love)

## Skills

| Skill | Description |
|-------|-------------|
| `drama-slider` | Personality scaling from 1 to infinity |
| `hales-ai-info` | Deep Hales AI company knowledge |
| `web-research` | Structured research with source evaluation |
| `code-wizard` | Modern coding patterns, solution-first |
| `vapi-telephony` | Voice agent integration |
| `n8n-automation` | Full workflow control |
| `mcp-bridge` | MCP server connectivity |

## Related Repos

- [notsoround/cupcake-opolis](https://github.com/notsoround/cupcake-opolis) — Forked OpenClaw runtime (Cupcake-branded)
- [notsoround/hales-ai-website](https://github.com/notsoround/hales-ai-website) — hales.ai website with Cupcake dashboard

## Security

- All credentials stored in `~/.openclaw/.env` (chmod 600, never committed)
- Telegram locked to owner ID only
- Web dashboard requires authentication
- Gateway binds to loopback only

## License

Private project by [Hales AI](https://hales.ai). Built on Valentine's Day 2026.

---

*Built with Claude Opus, powered by OpenClaw, fueled by chaos and cute bows.*
