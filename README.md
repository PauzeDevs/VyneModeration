# Vyne Moderation

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Inter&weight=600&size=22&duration=2600&pause=700&color=4C8DFF&center=true&vCenter=true&width=680&lines=Vyne+Moderation" alt="Animated header: Vyne Moderation">
</p>

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

Create a local `.env` file for runtime settings. The bot requires `DISCORD_TOKEN`, `CLIENT_ID`, and `GUILD_ID`. Optional AI settings are `GEMINI_API_KEY` and `GEMINI_MODEL`; the default model is `gemini-3.8-flash`. The hosting integration reads `BOT_HOSTING_API_KEY`, and `VYNE_OWNER_ID` can identify the owner. Music uses Lavalink settings `LAVALINK_ID`, `LAVALINK_HOST`, `LAVALINK_PORT`, `LAVALINK_PASSWORD`, and `LAVALINK_SECURE`. Optional report routing uses `VYNE_SUPPORT_GUILD_ID` and `VYNE_SUPPORT_REPORT_CHANNEL_ID`. The tracked [.env.example](.env.example) currently demonstrates the Lavalink settings.

Do not commit bot tokens, API keys, or other secrets.

## License

Vyne Moderation is distributed under the license included in this repository.
