# Token Forest — Privacy Notes 🔒

[English](PRIVACY.md) · [简体中文](PRIVACY.zh-CN.md)

Token Forest exists because we wanted a cozy way to *see* our own AI usage — not to collect anyone's data. This page explains, in plain language, exactly what the app touches.

## The one rule

**What happens on your machine stays on your machine.**

## What Token Forest reads

Claude Code and Codex already keep usage logs on your computer (that's how their own tools report usage). Token Forest reads **only the token counts** from those local files:

- input tokens, output tokens, cache-read tokens, cache-write tokens
- the model name and timestamp of each entry (for per-model stats and daily curves)

That's the whole list.

## What Token Forest never reads

- ❌ Your source code
- ❌ Your prompts or the AI's responses
- ❌ Your files, projects, or anything else on disk

The growth logic needs a number, not your novel. It only ever gets the number.

## What Token Forest stores

A few small local files next to the app: your tree's growth state, your settings (window position, language, etc.), and aggregated daily usage totals. All local. Delete them and the app starts fresh.

## Network access

**None, by default.** No telemetry, no analytics, no update pings, no price lookups (cost estimates use a built-in offline price table).

The **only** network feature is the **leaderboard**, and it is strictly opt-in:

| | |
| --- | --- |
| What's submitted | your chosen nickname, region, tree token total, growth stage |
| How you're identified | an anonymous account — no email, no name, no machine info |
| Opting out | turning the leaderboard off **deletes your entry** from the server |

## Verifying these claims

We take "trust us" seriously enough to know it isn't good enough. The source code is currently private, but we're exploring opening the core usage-reader component so these claims can be independently audited. Until then: the app works with your network disabled — try it.

## Questions?

Write to [contact@tokenforest.com.au](mailto:contact@tokenforest.com.au) — privacy questions get answered first.
