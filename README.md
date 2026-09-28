# Vyne Moderation

Vyne is a Discord moderation and server-management bot built with discord.js v14. It combines moderation, security, automation, community tooling, music, and optional AI features in a single bot.

## Features

- Moderation — bans, kicks, timeouts, warnings, purges, locks, and role management
- Security — AutoMod, Anti-Nuke, raid protection, and verification tooling
- Tickets — support workflows with configurable customization
- Welcome and VoiceMaster — onboarding and temporary voice channels
- Analytics and leveling
- Optional Gemini-powered AI
- Economy, giveaways, polls, and reminders
- Private member reporting to configured staff logs
- Premium and No-Prefix access systems
- Music through Lavalink

## Commands

- `/help` — interactive command center
- `/ping` — bot and WebSocket latency
- `/report @user reason` — send a private member report to staff
- `/logchannel #channel` — configure the staff log channel
- `/sys status` — inspect hosting status

The command set is intentionally modular and may evolve as features are added.

## Requirements

- Node.js `>= 22.12.0`
- Discord bot application and token
- Required Discord intents enabled for the features you use
- Optional Gemini API key for AI functionality
- Lavalink-compatible audio infrastructure for music

## Installation

```bash
npm install
```

Create `.env` with the required credentials and configuration, then start the bot:

```bash
npm start
```

Run the built-in syntax checks with:

```bash
npm test
```

## Stack

- Node.js / CommonJS
- discord.js v14
- `@discordjs/voice`
- `lavalink-client`
- Google GenAI
- `@napi-rs/canvas`
- dotenv

## Configuration

Keep credentials in environment variables. Do not commit bot tokens, API keys, or other secrets to the repository.

## License

Vyne Moderation is distributed under the license included in this repository.
