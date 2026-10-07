# Bellmont & Co. — Game Bible

Private source-of-truth repository for the Bellmont & Co. point-and-click game.

## Start here

1. Read `CURRENT_STATE.md`.
2. Read `canon/CANON_INDEX.md` and `canon/master_story_bible_v0_3.md`.
3. Read the relevant current file in `canon/`.
4. Read the matching implementation/scene brief in `production/`.
5. For any visual work involving an existing person or location, use the exact files in `references/` as references. Do not reconstruct them from prose.

## Authority order

1. User-supplied master story bible v0.3 for historical truth and future plot.
2. Current implemented build and exact line maps for playable scope; remaining current files in `canon/`.
3. Current files in `production/`.
4. Approved visual references in `references/`.
5. `archive/obsolete/` is historical only and must never override current canon.

## Locked rules

- Setting: USA, 1998, late autumn.
- Bellmont & Co. is a historic American department store from the early 20th century.
- The building has exactly 6 floors.
- **Bellmont & Co. is never translated.**
- In-world UI, signs, documents and dialogue are Russian unless a proper world name such as Bellmont & Co. is intentionally retained.
- No Russian/Soviet architectural look.
- Existing faces and locations are immutable visual references unless explicitly recast/redesigned.
- Do not infer canon from memory when a current repository file exists.
- When canon changes, update the relevant current file and `CURRENT_STATE.md` together.
- Superseded drafts belong in `archive/obsolete/`.

## Layout

- `canon/` — story, current dialogue and canon index.
- `production/` — current implementation handoffs and scene briefs.
- `references/characters/` — canonical character references.
- `references/locations/` — canonical location references.
- `archive/obsolete/` — superseded drafts only.
