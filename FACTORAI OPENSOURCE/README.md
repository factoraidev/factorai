# FactorAI Open Source Setup

This repository is prepared for open source sharing.

No real API keys should ever be committed. Use your own keys locally or in your deployment platform environment variables.

## Quick Start

1. Copy `.env.example` to `.env`.
2. Fill the placeholders in `.env` with your own credentials.
3. Run the project normally.

## Required Environment Variables

- `OPENAI_API_KEY`: Your OpenAI API key used by server endpoints.
- `OPENAI_MODEL`: OpenAI model name (default example: `gpt-4.1-mini`).
- `NEWS_PORT`: Local server port (default: `8787`).
- `TAVILY_API_KEYS`: One or multiple Tavily keys separated by commas.

Example:

`TAVILY_API_KEYS=key_one,key_two,key_three`

## Optional Environment Variables

- `TWITTER_API_KEY`
- `TWITTER_API_SECRET`
- `TWITTER_ACCESS_TOKEN`
- `TWITTER_ACCESS_TOKEN_SECRET`

These are only needed for X/Twitter posting features.

## Security Notes

- Never commit `.env` with real credentials.
- Rotate any key immediately if it was exposed before.
- Add secrets only in local `.env` or your cloud provider secret manager (for example Vercel Environment Variables).

