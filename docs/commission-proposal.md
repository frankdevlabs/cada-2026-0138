# Commission proposal — digest

- **Proposal:** `COM(2026) 502 final` (3 June 2026) — "establishing a framework of measures for
  strengthening Europe's cloud and AI ecosystem (Cloud and AI Development Act)", Text with EEA relevance
- **Legal bases:** Articles 114 and 173(3) TFEU
- **Accompanying:** SWD(2026) 502 (impact assessment, Parts 1–2), SWD(2026) 503 (executive summary), Annexes 1–3
- **Base-text extracts:** [`extracts/commission/`](../extracts/commission/) — transcribed (10 slices; anchors `article-N`)
- **Register entry:** [`sources/README.md`](../sources/README.md)

## Why (the Commission's case)

Per the explanatory memorandum and press material: the EU depends on non-EU providers for >80% of
digital products/services/infrastructure (Draghi report); produces <10% of global semiconductors; three
non-EU hyperscalers (AWS, Microsoft Azure, Google Cloud) hold >70% of the EU cloud market — the European
share shrank from 29% (2017) to 15% (2022); the EU spends ~€264bn/year largely on US proprietary IT.
EVP Virkkunen: "we want to be sure nobody has a kill switch". The Commission states the US CLOUD Act is
an obstacle for US providers to reach the highest assurance levels, and that the EU–US Data Privacy
Framework does not remove sovereignty concerns because "the notion of sovereignty goes beyond data
transfers and relates to operational autonomy too".

## Structure (48 articles, five Titles)

| Title | Articles | What it does |
|---|---|---|
| I — General provisions | 1–2 | Subject matter, definitions — [extracts](../extracts/commission/COM-2026-502_general-provisions-art1-2.md) |
| II — Research, development and deployment activities for the cloud and AI ecosystem | 3–9 | Cloud and AI Leadership Initiatives: objectives, Experience and Acceleration Centres for AI (built on the EDIHs), implementation mechanisms, national cloud-and-AI strategies (within 1 year of entry into force), frontier AI priority projects + compute allocation — [extracts](../extracts/commission/COM-2026-502_leadership-initiatives-art3-9.md) |
| III — Data centre capacities | 10–15 | Member-State **acceleration zones** (designation, conditions, single information points, facilitated permitting); Commission-designated **data centre strategic projects**; Union capacity-gap monitoring — [extracts](../extracts/commission/COM-2026-502_data-centres-art10-15.md) |
| IV — Autonomy | 16–44 | Ch I (16–28): **Union cloud sovereignty framework** — four assurance levels (requirements in Annex II), recognition via national competent authorities, third-country recognition ([Art 18](../extracts/commission/COM-2026-502_sovereignty-framework-art16-28.md#article-18)), self-assessment (level 1) vs third-party audit (levels 2–4), central repository, transparency, penalties, mutual assistance, cross-border enforcement — [extracts](../extracts/commission/COM-2026-502_sovereignty-framework-art16-28.md). Ch II "Demand-side measures" (29–33): public-sector **risk assessments**, minimum-level **procurement obligations** (level-1 floor; levels 2–4 where activities have public-order relevance), NIS2-sector private entities may run equivalent impact assessments, Union-added-value procurement criteria, innovation-procurement monitoring — [extracts](../extracts/commission/COM-2026-502_public-sector-use-art29-33.md). Ch III (34–36): **EuroCloud Federation** (public-sector cloud federation, service sharing, cost recovery) — [extracts](../extracts/commission/COM-2026-502_eurocloud-federation-art34-36.md). Ch IV (37–40): Commission **common procurement framework** (incl. Financial Regulation derogations, fee-based cost compensation) — [extracts](../extracts/commission/COM-2026-502_common-procurement-art37-40.md). Ch V (41–44): **open source** — preference obligation, sharing/reuse of publicly-developed software, EU Open Source Solutions Catalogue, network of OSPOs — [extracts](../extracts/commission/COM-2026-502_open-source-art41-44.md). *(The memorandum mislabels the open-source chapter "Chapter VI"; the operative text says Chapter V.)* |
| V — Final provisions | 45–48 | Delegated acts (45 — see drafting quirks below), implementing acts (46), review (47), entry into force/application (48) — [extracts](../extracts/commission/COM-2026-502_final-provisions-art45-48.md) |

CADA **amends and repeals nothing** — it is a standalone regulation that interfaces with the Data Act,
NIS2, DORA, GDPR, the AI Act and the Cybersecurity Act (see
[`instruments/related-instruments.md`](instruments/related-instruments.md)).

## Headline ambitions

- Triple EU data-centre capacity within 5–7 years (Union has the needed capacity by 2035); ~€200bn
  investment, mostly private.
- Public bodies in NIS2 sectors (digital infrastructure, energy, research, health) and in national
  security/defence/border/justice/law-enforcement functions restricted to assurance levels 2–4
  depending on sensitivity.
- The framework leaves room for national "à la carte" application (not fully harmonised) — see
  [`fault-lines.md`](fault-lines.md).
- The Commission may, via implementing acts, require private NIS2-sector entities to run comparable
  assessments, and identify third countries whose providers can be assessed against the framework.

## Drafting quirks in the source

Observed while transcribing the operative text (all preserved verbatim in the extracts, flagged inline):

- **Title V numbering slip:** the delegation article is printed "**Article 44**" — duplicating the
  Chapter V OSPO article's number — while every cross-reference in the Regulation ("delegated acts in
  accordance with Article 45": Arts 6(4), 16(2), 20(9), 21(1), 31(3)) and the memorandum call it
  **Article 45**; there is no printed Article 45 — [extract (anchor `article-44-bis`)](../extracts/commission/COM-2026-502_final-provisions-art45-48.md#article-44-bis).
- **Article 2 definitions skip points (23)–(24)** — [extract](../extracts/commission/COM-2026-502_general-provisions-art1-2.md#article-2).
- **Art 30(4)** points are labelled (a), (b), (a) — the third point is mislabelled — [extract](../extracts/commission/COM-2026-502_public-sector-use-art29-33.md#article-30).
- **Art 40(5)** has a duplicated paragraph number ("5. 5.") and near-duplicate points (c)/(d) — [extract](../extracts/commission/COM-2026-502_common-procurement-art37-40.md#article-40).
- **Art 34(3)** point list ends at (b) with a trailing semicolon — possible truncation — [extract](../extracts/commission/COM-2026-502_eurocloud-federation-art34-36.md#article-34).
- The memorandum mislabels the open-source chapter ("Chapter VI"; operative text: **Chapter V**).
- Scattered typos kept verbatim (e.g. "subpragraph", "review perioed", "theirflexibility", "buiying"
  in a recital, "pursuant Decision" missing "to"); Art 38(9) cites "Regulation (EU, Euratom)
  **2014/2509**", an apparent typo for 2024/2509.

These are the kind of points a first Presidency compromise text typically cleans up — useful markers
for diffing the first ST version.

> Figures are cited from the proposal/press material; provision-level statements can now be verified
> against the operative text in [`extracts/commission/`](../extracts/commission/) (working
> transcriptions — cross-check the committed PDF before relying on them).
