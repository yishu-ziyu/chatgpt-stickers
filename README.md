# ChatGPT Stickers

A personal reaction-image library curated for ChatGPT conversations.

The important rule is simple: **ChatGPT owns the curation work.** The user does not need to keep feeding the library manually. When a conversational gap appears, the assistant can source or create a better reaction image, tag it, and add it to the library.

## Current starter pack

The library starts with 24 broadly useful reaction assets covering:
- laughter / absurdity
- surprise / disbelief
- thinking / skepticism
- speechlessness / awkwardness
- celebration / approval
- curiosity / watching
- playful frustration
- polite or dry reactions

The starter pack uses Twemoji assets. Future additions should prefer original, public-domain, or clearly open-licensed sources.

## Structure

- `stickers/index.json` — semantic metadata, source/license info, and render URLs
- `CHATGPT.md` — proactive usage and sourcing rules
- `stickers/` — optional locally stored assets

## How selection works

ChatGPT matches the current conversation against each asset's:
`emotion`, `tone`, `tags`, `usage`, `aliases`, and `intensity`.

The goal is not to maximize the number of stickers. The goal is to have a small library with good semantic coverage, then expand only when real conversations expose gaps.

## Attribution

Twemoji graphics © Twitter, Inc. and other contributors, licensed under CC BY 4.0.
Source: https://github.com/twitter/twemoji
