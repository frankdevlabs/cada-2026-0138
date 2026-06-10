# Transcription guide for Commission base-text extracts

Internal standard for every file in `extracts/commission/`. The goal: a faithful, diffable
transcription of the **operative text of the Commission proposal COM(2026) 502 final** (CELEX
52026PC0502), structured to line up with the Council extracts in `../council/` so that
`git diff --no-index ../commission/COM-2026-502_<slice>.md ../council/ST-<nnnn>-<yyyy>_<slice>.md`
is meaningful.

## Source of truth
The committed proposal under `../../sources/commission/COM-2026-502_proposal_2026-06-03.pdf` (the
enacting articles and recitals), cross-checked against the authoritative EUR-Lex copy
(CELEX **52026PC0502**). The annexes (incl. **Annex II**, the assurance-level requirements) are
`../../sources/commission/COM-2026-502_annexes-1-3_2026-06-03.pdf`. Transcribe from the committed
source on disk; never from memory or a web summary.

## This is the baseline — there are no tracked changes
The Commission proposal is the **original**: there is nothing to "consolidate". CADA is a
**standalone regulation** (it amends/repeals nothing), so — unlike amending-instrument files — there
are no amending instructions either: transcribe the articles **verbatim as enacted text**. Where an
article interfaces with existing law (NIS2 sectors, Cybersecurity Act certification, Financial
Regulation derogations), flag it with a `▸` note linking the relevant
`../../docs/instruments/related-instruments.md` row, and — once Council versions exist — what the
Council did to that point, linking the matching `../council/` anchor.

## Faithfulness rules (hard)
- Transcribe operative wording verbatim. This is primary legal text, not prose to paraphrase.
- Preserve the proposal's own article/paragraph numbering and Title/Chapter/Section structure.
- Preserve bracketed placeholders exactly — e.g. `[OP: please insert the date = … after entry into
  force]` — that is *not* `[illegible]`; it is undecided in the source.
- If a passage is genuinely illegible/uncertain in the source, mark it `[illegible in source]` — never
  guess.

## Structure & anchors
- One file per slice in [`../../tracker.yaml`](../../tracker.yaml) `extract_slices`, named
  `COM-2026-502_<slice>.md`. The slices follow the proposal's own Title/Chapter groupings
  (Title I Arts 1–2; Title II Arts 3–9; Title III Arts 10–15; Title IV ch I Arts 16–28, ch II
  Arts 29–33, ch III Arts 34–36, ch IV Arts 37–40, ch VI Arts 41–44; Title V Arts 45–48; recitals).
  Confirm the groupings against the text while transcribing and adjust `extract_slices` if the
  proposal's own structure differs.
- Anchor every article heading with `<a id="article-N"></a>` (exactly `article-N` — no topic suffix;
  recitals use `recital-N`), so future Council versions can reuse the anchors and cross-version diffs
  line up. Sole exception: Title V's misprinted second "Article 44" carries `article-44-bis`.
- Recitals file: curated subset (the contested/structural ones). State that it is a curated subset,
  not the full preamble.

## Header block (every file)
Open with a blockquote: source = **COM(2026) 502 final**, 3 June 2026, interinstitutional file
**2026/0138 (COD)**, "working transcription, not an official text", "verify against the authoritative
document (EUR-Lex CELEX 52026PC0502)", and "See `../../NOTICE`."

## Cross-links
Relative links only. Link the sibling extracts, the matching `../council/` anchors (once they exist),
and the relevant `../../docs/provisions/*` / `../../docs/instruments/*` pages. Verify every internal
link/anchor resolves (`python3 ../../.claude/skills/transcribe-council-extract/linkcheck.py ../..`)
before finishing.
