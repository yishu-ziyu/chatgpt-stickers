# ChatGPT Sticker Rules

When the user asks for a sticker / reaction image, or when a sticker would clearly improve a casual conversational moment:

1. Read `stickers/index.json`.
2. Match the user's intent semantically against `tags`, `emotion`, `tone`, `usage`, and `aliases`.
3. Prefer the single best match. Do not dump multiple stickers unless the user asks to choose.
4. Render the sticker directly using its `url`.
5. Do not use a sticker in serious, vulnerable, medical, legal, safety-critical, grief, or distress contexts.
6. If no good match exists, say that the library has no suitable sticker yet instead of forcing one.
7. When the user provides a new sticker and asks to save it, store the image under `stickers/` and add metadata to the index.

Recommended response form:

`![sticker](<url>)`

Keep any accompanying text brief.
