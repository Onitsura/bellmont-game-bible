# CURRENT STATE

**Updated:** 2026-10-02  
**Playable build checked:** `Bellmont_Co_Chapter3_Furniture_v7_1_final.zip` (Godot 4.6).

## Canon and authority

`canon/expanded_game_skeleton.md` defines the expanded full-game structure, three investigation lines and later plot. For the actual Chapter 3 route, `canon/chapter3_identity_without_caption.md` records the implemented details and supersedes conflicting Chapter 3 planning beats in the older skeleton. `canon/dialogue_current_build.md` holds exact dialogue text and states the separate provenance of legacy voiced lines and newly added text-only lines. Open questions in section 14 of the skeleton remain open.

The hidden long-form truth is not all available to the player at this point. In particular, the current build has established neither why Nora left nor her true return journey, and it has not proved what happened to the employee-fund money.

## Implemented through

The playable route now extends beyond the box and Victoria conversation:

- Prologue, lobby, archive, journal `ГАРАНТИЯ → IV / VI / II → 462`, missing agreement №317, second floor with Amelia, internal phone `14`, Thomas and the freight elevator sequence `1 → 3 → 6 → 7`, the 1958 box and the Victoria conversation.
- **Chapter 2 / anniversary materials:** lower cabinet at the reference desk, five alternative period packets laid out on the same table, the 1908–1958 jubilee packet, booklet, program, group and reception photographs, jubilee newspaper and later departure clipping. The player sees that the newspaper caption misidentifies the woman as Evelyn; her actual name remains unknown here. Group photograph reverse: 17.10.1958, series 6, frame 4, swallow-in-oval mark. See the entrance to `canon/chapter3_identity_without_caption.md`.
- **Chapter 3 / identity without a caption:** Amelia's auction ledger and furniture lots, middle passenger lift to fourth floor, four visible states of the blocked personnel corridor (strap, boxes, cabinet), photo-service log and sleeves, four sliding card tracks, real wrong drawers and correct `Ф-2 / Л-7`, 12-frame sheet, frame 8 → employee № 0418, Nora Keller's official personnel card, department code `4-С`, and Thomas's conversation at the second-floor freight lift. Details and exact evidence gates: `canon/chapter3_identity_without_caption.md`.

The v7.1 Chapter 3 Amelia/Thomas dialogue is text-only; older spoken lines remain in the build. New voice recordings and final human visual playtest are still pending. The automatic Chapter 3 route and corridor-state checks passed (`CHAPTER3_FULL_ROUTE_PASS`, `CORRIDOR_FOUR_STATES_PASS`); this is not a measured 30–40 minute human playthrough.

## Current player knowledge at the end of Chapter 3

- The woman in the later newspaper is **Nora Keller**, employee № 0418, associated with the old department code **4-С** (расчётно-фондовый сектор).
- Thomas says Nora was his mother and that he recognized her handwriting on the box note. He had concealed that recognition.
- Thomas was told she died during a trip. He does not know why she went. The player has **not** proved a connection between Nora's work, the expense document for **$184,620.47**, and the old agreement.
- There are six floors. The freight indicator's `7` and key `Т2-17` remain unresolved.

## Next production block

**Chapter 4 — the financial trail** under the expanded skeleton. First produce a detailed 30–40 minute active-gameplay design: interactions, branches, dialogue, a substantial document/accounting puzzle and coherent reference images of locations, objects and puzzle states. Show the proposed images and interaction material for approval **before implementation**. Do not treat proposed Chapter 4 visuals or text as assets already in v7.1. The later canon establishes an unpaid remainder of the protected employee fund; Chapter 4 must assemble that conclusion from records without prematurely revealing the full terms of agreement №317.

## Visual source of truth

The user-supplied Bellmont exterior and character references for Charles, Nora and Evelyn, plus `references/characters/CHARACTER_VISUAL_CANON.md`, anchor existing faces. Amelia's current short bob / каре is required in both scene and dialogue portraits. Existing architecture and unhandled props should stay consistent between views and interaction states. The setting is an American department store in 1998, late autumn, at dusk; exactly six floors. No city labels without explicit canon; **Bellmont & Co.** remains untranslated, and the family name in Russian is **Беллмонт**.

## Audio

Production decision: Eva — generated voice; Victoria, Thomas, Amelia and other principal NPCs — live actors. Older clips may remain as placeholders. New dialogue needs stable audio IDs before recording or ingest; Chapter 3's technical sequence labels in the dialogue file are **not** recorded audio IDs. See `production/voice/voice_implementation.md` for implementation notes, with any older casting notes reconciled against this decision.
