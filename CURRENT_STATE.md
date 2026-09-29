# CURRENT STATE

**Updated:** 2026-09-29

## Master expanded canon

The project has moved from a mostly linear Day 1 structure to the expanded investigation structure in `canon/expanded_game_skeleton.md`.

That file is now the master canon for:
- the full chapter structure;
- the three post-box investigation lines (identity / money / building);
- repeated use of locations and inventory;
- the major puzzle chain and cross-links between clues;
- the route toward Nora, the employee-fund investigation, T2-17, Arthur/Leonard, Evelyn's final route and Agreement №317.

The currently implemented route through the box and Victoria conversation remains intact as the prologue / Chapter 1. Exact implemented dialogue is not silently rewritten by the expanded skeleton.

Details explicitly listed as open in section 14 of the expanded skeleton remain undecided until separately approved.

## Implemented through

Current playable build is implemented through the freight-elevator box discovery and the subsequent conversation with Victoria about the box contents.

Implemented route includes:

- intro;
- lobby / first Victoria conversation;
- Thomas and service corridor;
- archive puzzle;
- `ГАРАНТИЯ → IV / VI / II → 462`;
- missing archive folder №317 and card marked `ВЫДАНО`;
- Victoria opens access to second floor;
- Amelia;
- flashlight;
- internal phone extension `14`;
- Thomas arrives at the old freight elevator;
- elevator test `1 → 3 → 6 → 7`;
- box from 1958;
- note, expense document, half photograph and key;
- Victoria conversation after the box.

## Current development block

**Reference desk / 1958 anniversary materials.**

Current interaction concept:

`1958 material set → interactive table → free inspection of booklet / program / photographs / group photograph / newspaper clippings → false public story about Evelyn's departure → visual contradiction.`

## Current locked story facts for this block

- Victoria already identified the woman on the half-photo as Evelyn.
- The anniversary set concerns Bellmont & Co.'s 50th anniversary in 1958.
- Charles Bellmont must appear in official anniversary materials.
- The group photograph contains Charles, Evelyn, Nora and many employees.
- Nora must be memorable in the group shot without being staged as a VIP or shoved into the foreground.
- The player does **not** know Nora's name yet.
- A newspaper later shows Nora but identifies her as Evelyn Bellmont.
- The article reports the departure of the woman it calls Evelyn after the anniversary week.
- Therefore the old public story of “Evelyn's departure” becomes suspicious.
- Do not reveal Nora's name, Nora/Thomas relationship, the employee fund truth, T2-17, or the meaning of 7 at this stage.

## Visual source-of-truth

Canonical references currently supplied by the user:

- Bellmont exterior;
- Charles Bellmont;
- Nora Keller;
- Evelyn Bellmont.

Rules:
- use the exact face references for future images;
- do not regenerate a merely “similar” person;
- no geographic city labels unless canon explicitly establishes one;
- Bellmont & Co. remains untranslated everywhere;
- period group photographs must look socially plausible: executives/family are central, ordinary employees are not inexplicably placed in VIP positions;
- Nora should be recognizable through subtle composition/wardrobe/gaze/background separation, not explicit highlighting.

## Audio

Current production decision:
- **Eva** — generated voice;
- **Victoria, Thomas, Amelia and other principal NPCs** — live actors rather than generated voices.

The current build may still contain previously generated placeholder/legacy clips. New dialogue production should use stable line IDs so live actor files and Eva generation can be replaced/updated without changing dialogue logic.

See `production/voice/voice_implementation.md` for implementation details; casting notes there may require reconciliation with this current decision.

## Next work

Implement **Chapter 2 — 1958 anniversary materials** as the first production block under the expanded master skeleton:

- locate the anniversary set at the reference desk;
- build the interactive materials table;
- let the player inspect booklet / program / photographs / group photograph / newspaper clippings in a non-linear order;
- confirm Evelyn independently;
- reach the visual contradiction: the newspaper woman is not Evelyn;
- preserve the three wider investigation lines without prematurely resolving Nora, the money trail or T2-17.

## Visual reference reconciliation — 2026-09-29

Reviewed the latest user-supplied character boards against project history.

Current identity anchors now recorded in `references/characters/CHARACTER_VISUAL_CANON.md`:
- Evelyn;
- Nora;
- Charles;
- Victoria;
- Leonard Crane (visual reference only unless story canon explicitly uses him);
- Thomas;
- Amelia.

**Amelia correction:** the older curly/long-hair character board is not current canon. On 2026-09-28 the user approved Amelia with a short bob / каре and required the large dialogue portrait and emotion states to preserve that hairstyle. Use the bob-hair master as the identity/silhouette source.

For Victoria, the newly supplied board is the face/identity anchor. Older in-game pose art may be used for pose/gesture reference only if facial details drift from the board.
