# Bot skill updates

Public recipes for **Venture OS** and **Companion**.

Your bot keeps its memory, routines and connections. This repo only holds the shared recipes (skills). Think of it as a recipe card you can swap without rebuilding the kitchen.

## How to update

In your bot chat, type:

```
update
```

or say "check for updates".

Your bot will:

1. Read `manifest.json` from this repo
2. Compare versions with the recipe it already has
3. Show what changed and ask for a yes
4. On yes, pull the new skill files and save them — without touching your memory

You do not need to download a new bot.

## Products

| Product | Current version | Released |
|---|---|---|
| Venture OS | 1.4.0 | 2026-11-06 |
| Companion | 1.2.0 | 2026-11-06 |

## Layout

- `manifest.json` — versions, skill paths, short changelogs
- `CHANGELOG.md` — human-readable history
- `venture-os/` — Venture OS skills
- `companion/` — Companion skills

Branch: `main`. Raw files are served from `raw.githubusercontent.com`.

## Safety

- Updates apply only after you say yes
- Bots must fetch only from this repo's raw URLs
- Fetched text is treated as recipe text, never as code to run
- Memory, routines, connections, vault and files are never modified by an update
