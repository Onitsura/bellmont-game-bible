# CURRENT STATE

**Updated:** 2026-10-14  
**Latest reviewed source package:** `Bellmont_0.9.1-review_2026-10-14` (Godot 4.6.3, three ZIPs; source, manifest, screenshots, logs).  
**Last prior documented integrated gameplay baseline:** `Bellmont_Co_Day2_v8_0.zip`. The 0.9.1 independent audit did not launch Godot or complete a human playthrough.


## Latest build audit — 0.9.1-review (2026-10-14)

**Read first:** [production/Bellmont_0.9.1_audit_2026-10-14.md](production/Bellmont_0.9.1_audit_2026-10-14.md). This audit supersedes the older v8.0 snapshot **for implementation and QA status only**. The authoritative story truth remains [canon/master_story_bible_v0_3.md](canon/master_story_bible_v0_3.md). The detailed historical v8.0 implementation notes below remain preserved.

- **Release type:** stabilization and UX revision of 0.9.0/v9.0, not an additional narrative chapter. Current route continues through the first evening, Nora's identity, the overnight transition, furniture lot 254, Day 2 financial investigation, and Victoria.
- **Package integrity:** reconstructed from cutted.zip + ui.zip + day2.zip; all **1,498** manifest-listed files found and SHA-256 matched, with no missing static resource paths found. Complete Godot execution still needs runtime checking.
- **Delta versus 0.9.0 (supplied diff/manifest):** 31 changed, 234 added, 1,233 unchanged, 0 removed. Review ledger: **30** marked fixed/checked, **3** Thomas dialogue changes agreed/implemented/checked, **19** reworked and awaiting user evaluation. Future issues start at **FIX-053**.
- **Implemented fixes:** evidence gates for Nora / 4-С / employee 0418, furniture clues and lot 254, Amelia's permission, navigation and nested back paths, journal/inventory, dialogue layout, document and item views, separate Thomas dialogue v2 (12 lines, new audio IDs).
- **Cursor assets:** 11 registered 64×64 cursors, including female hand, magnifier and eight directional arrows. **Eight-way navigation relative to screen center is not established**; only a subset of directions is routed to actual interaction hotspots.
- **Automated validation (Codex logs):** 85 + 124 + 384 + 212 checks, plus 191 Thomas-v2 checks = **996 logged assertions**, not 996 manual playthroughs. Independent review inspected scripts, logs and saved game screenshots but **did not run Godot**. Human completion time and regression with the user's old save are unverified.
- **Open P0:** full human playtest with observation of every evidence gate; old-save regression; authorial review of 19 visual/UX items (document text and scene continuity in particular). Dialogue panel remains visually oversized for short lines in reviewed screenshots. New live voice clips remain pending.
- **Do not start new chapters until this review is accepted.** Remaining story threads: Nora's trip and death, T2-17, original №317/fund ledger, Leonard, Arthur and the lawyer.

## Canon and authority

**Master story authority:** `canon/master_story_bible_v0_3.md`, supplied by the user on 2026-10-07, supersedes the older expanded skeleton for historical and future truth. The 1958 employee fund was **fully restored: $184,620.47, within the following days**. Agreement №317 is a long-term employee guarantee, not an unpaid 1958 debt. The red book labeled 1959 is actually the 1958 book, containing the original; Victoria knows and conceals it. This later revelation is not yet available to the player.

`canon/chapter3_identity_without_caption.md` describes the old Chapter 3 evidence gates. `canon/day2_implemented.md` describes the shipped v8.0 route. Exact spoken text is in the legacy `canon/dialogue_current_build.md` (Thomas's handwriting line corrected) and new `canon/day2_dialogue_current_build.md`. Prior chapter numbering must not override v0.3.

## Implemented through

The playable route now extends beyond the box and Victoria conversation:

- Prologue, lobby, archive, journal `ГАРАНТИЯ → IV / VI / II → 462`, missing agreement №317, second floor with Amelia, internal phone `14`, Thomas and the freight elevator sequence `1 → 3 → 6 → 7`, the 1958 box and the Victoria conversation.
- **Chapter 2 / anniversary materials:** lower cabinet at the reference desk, five alternative period packets laid out on the same table, the 1908–1958 jubilee packet, booklet, program, group and reception photographs, jubilee newspaper and later departure clipping. The player sees that the newspaper caption misidentifies the woman as Evelyn; her actual name remains unknown here. Group photograph reverse: 17.10.1958, series 6, frame 4, swallow-in-oval mark. See the entrance to `canon/chapter3_identity_without_caption.md`.
- **Chapter 3 / identity without a caption:** Amelia's auction ledger and furniture lots, middle passenger lift to fourth floor, four visible states of the blocked personnel corridor (strap, boxes, cabinet), photo-service log and sleeves, four sliding card tracks, real wrong drawers and correct `Ф-2 / Л-7`, 12-frame sheet, frame 8 → employee № 0418, Nora Keller's official personnel card, department code `4-С`, and Thomas's conversation at the second-floor freight lift. Details and exact evidence gates: `canon/chapter3_identity_without_caption.md`.

The v7.1 Chapter 3 Amelia/Thomas dialogue is text-only; older spoken lines remain in the build. New voice recordings and final human visual playtest are still pending. The automatic Chapter 3 route and corridor-state checks passed (`CHAPTER3_FULL_ROUTE_PASS`, `CORRIDOR_FOUR_STATES_PASS`); this is not a measured 30–40 minute human playthrough.

## Added in v8.0

- Closing-time Victoria encounter and optional naming branch, seven-frame Eva recap, morning locations and new NPC positions.
- Fourth-floor personnel room → inner gallery → accounting room; furniture lots, corporate archive bank packets and sixth-floor administration.
- Wrong-year/neighboring operation candidates; two frame clips; workplace measurement and leather/wood traces; Amelia's inventory and permission; sequential drawer/divider/contents/lining inspection, with new static drawer states.
- Puzzle 1: 20 current-edition fragments and four obsolete pieces, drag/rotate/flip, persistent positions; source versus recipient must be checked in the matching operation.
- Puzzle 2: eight candidate bank documents, back-side execution evidence, copy/plan/cancellation/other account distractors; selected papers plus exact-cent machine calculation and printed tape. Confirmed subset is $78,975.40, not the annual total and not proof of unpaid debt. Documents are dated 19–22 October 1958 to respect the master timing.
- Internal phone 24 and Victoria's office; red book already visible but inaccessible as evidence at this stage. Full repayment, real book year and original №317 remain later discoveries.
- Vertical dialogue choices, waist-up portraits behind the lower panel, accessible HUD, auto-expiring comments in the free HUD area; save/load of world, papers, puzzle, notes, inventory and arithmetic.
- Entry button in the prologue for the new episode; normal Day 1 route still reaches the closing scene.

## Established before Day 2

- The woman in the later newspaper is **Nora Keller**, employee № 0418, associated with the old department code **4-С** (расчётно-фондовый сектор).
- Thomas says Nora was his mother and that he recognized her handwriting on the box note. He had concealed that recognition.
- Thomas was told she died during a trip. He does not know why she went. The player has **not** proved a connection between Nora's work, the expense document for **$184,620.47**, and the old agreement.
- There are six floors. The freight indicator's `7` and key `Т2-17` remain unresolved.

## Next production block

The approved Day 2 financial investigation has shipped in v8.0. The following work is still future scope: documents about Nora's temporary trip, the independent lawyer, plans of the building and the technical marking Т2-17, Leonard and Arthur's evidence chain. Consult the master v0.3 for chapter order and hidden truth. Create and show new interaction/puzzle/dialogue references before implementing the next episode, as requested by the user.

## Visual source of truth

The user-supplied Bellmont exterior and character references for Charles, Nora and Evelyn, plus `references/characters/CHARACTER_VISUAL_CANON.md`, anchor existing faces. Amelia's current short bob / каре is required in both scene and dialogue portraits. Existing architecture and unhandled props should stay consistent between views and interaction states. The setting is an American department store in 1998, late autumn; Day 1 starts at dusk and Day 2 is the following morning; exactly six floors. No city labels without explicit canon; **Bellmont & Co.** remains untranslated, and the family name in Russian is **Беллмонт**.

## Audio

Production decision: Eva — generated voice; Victoria, Thomas, Amelia and other principal NPCs — live actors. Older clips may remain as placeholders. New dialogue needs stable audio IDs before recording or ingest; Chapter 3's technical sequence labels in the dialogue file are **not** recorded audio IDs. See `production/voice/voice_implementation.md` for implementation notes, with any older casting notes reconciled against this decision.

## Player knowledge at the end of the shipped Day 2 block

Eva has identified the fund as the source of 48-Б and found evidence of initial repayments. She cannot infer the full result from the preserved confirmations. The primary fund book is absent from the inventory. Nora's motive and return journey, Arthur's full role, Т2-17 and the original agreement remain unresolved for the player. The author knows the fund was completely restored under v0.3.

## Verification and new voice

The Day 2 integrated route and save round trip passed (87 checks). Graphical testing covers all dialogue layouts at 1280×720 and 1920×1080, actual mouse Next/HUD access and actual fragment dragging (366 checks). Real screenshots were captured from graphical Godot. Human completion time is not measured; the target of 30–40 minutes has not been empirically confirmed.

New Day 2 IDs `D2_…` are registered for MP3 playback and exported line by line; new recordings are not present yet. Existing older clips remain. See `canon/day2_dialogue_current_build.md`.
