---
name: n8n-automation
description: Control n8n workflows on automate.hales.ai — trigger email, calendar, contacts, TTS, and custom automations
version: 1.0.0
author: Cupcake
---

# n8n Workflow Automation

You have access to a full n8n automation platform at `https://automate.hales.ai`.

## Available Workflows

### Active & Ready
| Workflow | ID | What it does |
|---|---|---|
| emailAgent | PSdLSuJ8af9aN9A0 | Full Gmail: send, receive, draft, reply, label |
| calendarAgent | elMct85LDcBxyJko | Google Calendar: create, get, update, delete events |
| contactAgent | dyiWb5zlU9LrEO9D | Airtable contacts: search, add, update |
| contentCreator | 5Up71prk8fblv8hM | Blog writer with Tavily research + Claude |
| ultimateAssistant | WvQ7eBF8VkDcaxLl | Orchestrator that routes to all sub-agents |
| ElevenLabs TTS | VD1ThpYnaHPULBaU | Text-to-speech at webhook/generate-voice |
| Cupcake Voice Bridge | wI5F001Io6nOH4Vt | Vapi voice → Telegram relay |
| Cupcake Web API | BE4mSVyET3yVyl10 | Web dashboard → command routing |

### Email Commands
- Check inbox: fetch latest emails from matt@hales.ai
- Send email: compose and send via Gmail
- Reply to email: reply to specific threads
- Draft email: save as draft for review

### Calendar Commands  
- Show today: list today's events
- Create event: schedule new calendar events
- Update event: modify existing events

### Voice Commands
- Call Matt: trigger outbound Vapi call to ${MATT_PHONE}
- TTS: generate speech via ElevenLabs

## API Details
- n8n Base URL: https://automate.hales.ai
- Webhook base: https://automate.hales.ai/webhook/
- Auth: API key in env (N8N_API_KEY)
- Matt's Gmail: matt@hales.ai
- Matt's Telegram ID: stored in env
- Matt's Phone: stored in env (MATT_PHONE)
