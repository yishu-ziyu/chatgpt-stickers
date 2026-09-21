# ChatGPT Stickers

A tiny personal sticker library for ChatGPT conversations.

The repository keeps sticker images plus a semantic index so ChatGPT can choose an appropriate sticker by meaning instead of by filename.

## Structure

- `stickers/` — image files
- `stickers/index.json` — semantic metadata and CDN URLs
- `CHATGPT.md` — usage rules for ChatGPT

## CDN

Public images can be served through jsDelivr:

`https://cdn.jsdelivr.net/gh/yishu-ziyu/chatgpt-stickers@main/stickers/<filename>`

## Add a sticker

1. Put the image in `stickers/`.
2. Add one entry to `stickers/index.json`.
3. Give it short tags describing emotion, tone, situation, and intensity.

The index is intentionally simple so it can be searched quickly in a normal ChatGPT conversation.
