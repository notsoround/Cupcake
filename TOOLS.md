# TOOLS.md - Cupcake's Local Notes

## Infrastructure

### Digital Ocean
- Droplet IP: 134.199.239.171
- hales.ai hosted on same droplet
- n8n (workflow automation) on same droplet: https://automate.hales.ai
- Cupcake deployment target: same droplet or dedicated

### AI Providers (via OpenRouter)
- **Primary:** DeepSeek R1 (reasoning) -- `openrouter/deepseek/deepseek-r1`
- **Fast:** DeepSeek V3.2, Grok 4.1 Fast
- **Multimodal:** Kimi K2.5, Gemini 3 Flash
- **Image Gen:** Nano Banana Pro, Nano Banana, Seedream 4.5, GPT-5 Image Mini
- **Fallback:** Qwen3 235B, local Ollama (when configured)

### Messaging
- **Telegram:** @CupcakeApocalypseBot (bot token in ~/.openclaw/.env)
- **WhatsApp:** Future addition

### Voice (Vapi.ai)
- Phone: +1 (872) 666-9598
- Assistant ID: ef458c7a-ba2e-49f6-97a2-f455c54978f7
- Voice: Savannah (11Labs)
- Model: DeepSeek V3.2 via OpenRouter
- Tool: cupcake_command -> n8n webhook -> Telegram

### n8n Workflow Automation
- URL: https://automate.hales.ai
- Cupcake workflow ID: wI5F001Io6nOH4Vt
- Webhook: https://automate.hales.ai/webhook/vapi-cupcake-hook
- Pipeline: Vapi voice call -> n8n webhook -> parse command -> Telegram message -> response to Vapi
- 27 total workflows on instance (Vapi, Telegram, ElevenLabs, email agents, etc.)

## Hales AI Website
- URL: https://hales.ai
- React/Vite/TypeScript SPA with Tailwind + Framer Motion
- Cupcake test page: /cupcake-test (PR #1 pending)
- GitHub: notsoround/hales-ai-website

## GitHub
- Account: notsoround
- Cupcake fork: notsoround/cupcake-opolis
- Website repo: notsoround/hales-ai-website

## Preferences
- IDE: Cursor
- Backup AI: Grok/Ara (unhinged mode available)
- Style: Fast, modern, no legacy patterns

## Credentials Location
All keys stored in `~/.openclaw/.env` (chmod 600):
- OPENROUTER_API_KEY, TELEGRAM_BOT_TOKEN, VAPI_API_KEY
- GITHUB_WEBSITE_TOKEN, N8N_API_KEY, N8N_BASE_URL
- VAPI_PHONE_NUMBER_ID, VAPI_ASSISTANT_ID, MATT_PHONE
