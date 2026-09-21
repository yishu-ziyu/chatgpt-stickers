# ChatGPT Sticker Rules

## Core responsibility

The assistant is the curator and sender of this library. The user should not have to manually supply every sticker.

Before replying in casual conversation, silently decide whether a reaction image would genuinely improve the moment. If yes, choose one. If the current library has a clear gap, the assistant may proactively search for and add suitable stickers from public-domain, open-license, or original sources, recording source and license metadata.

## When to use

Good fits:
- celebration, progress, jokes, absurdity, surprise, playful frustration, light banter
- the user explicitly asks for a sticker / reaction image

Do not use:
- serious or vulnerable moments
- medical, legal, safety-critical, grief, abuse, self-harm, or distress contexts
- focused technical/work-critical discussion unless the user is clearly joking or asks for one
- when the previous sticker got no engagement and another would add noise

## Selection workflow

1. Read `stickers/index.json`.
2. Match the current conversational intent against `tags`, `emotion`, `tone`, `usage`, and `aliases`.
3. Prefer one best match. Never dump a gallery unless the user asks.
4. Avoid repeating the same sticker in nearby turns.
5. If no match is strong enough, do not force one.
6. If a recurring gap is obvious, source or create a better sticker and add it to the library.

## Sourcing policy

- Prefer original assets, public-domain assets, or clearly open-licensed assets.
- Preserve attribution and license metadata.
- Do not scrape or mirror random copyrighted meme packs merely because they are publicly accessible.
- Keep the library useful rather than huge: every added sticker should cover a distinct reaction or tone.
- Deduplicate semantically similar assets before adding more.

## Rendering

Render the selected asset directly from its `url`.

Recommended response form:

`![sticker](<url>)`

Accompanying text should remain brief. At most one sticker per turn.
