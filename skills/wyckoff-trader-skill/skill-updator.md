# Skill Updator

Use this process whenever new Wyckoff or crypto-market material needs to be folded into `wyckoff-trader-skill`.

## Objective

Update the skill without bloating `SKILL.md`, losing old insights, or duplicating the same concept in multiple places.

## Update Workflow

### 1. Register The New Source

For each new source, note:

- title
- author
- date
- URL or file path
- source type: book, blog, report, course notes, thread, video transcript
- why it matters

Then update `references/source_index.md`.

If the source text is not already bundled locally, also add a simplified local copy under `references/assets/`.

If the source is a large recurring archive, also create a corpus-level `index.md` and `manifest.json` inside its asset folder.

### 2. Extract Only High-Signal Ideas

Do not copy the whole source into the skill.

Instead, pull out:

- new concepts not already covered
- better definitions of existing concepts
- crypto-specific adaptations
- scenario-building heuristics
- trade-location logic
- intermarket or rotation rules

Ignore:

- generic motivational language
- repeated textbook definitions
- low-signal market recaps
- promotional content

### 3. Decide Where The Insight Belongs

Use this routing:

- formal Wyckoff framework -> `references/book_foundations.md`
- crypto-specific behavior -> `references/crypto_adaptations.md`
- unusual or easy-to-miss ideas -> `references/uncommon_concepts.md`
- scenario-output or workflow changes -> `references/scenario_playbook.md`
- trigger conditions or workflow navigation -> `SKILL.md`
- local source text or offline corpus material -> `references/assets/`
- source-family distilled takeaways -> a dedicated reference file such as `references/<source_family>.md`

## Editing Rules

- Keep `SKILL.md` procedural and short.
- Prefer adding detail to `references/` instead of expanding `SKILL.md`.
- Avoid duplicate explanations across files.
- If a new idea changes how scenarios should be built, update both the relevant reference file and the workflow wording in `SKILL.md`.
- Keep source assets simplified and local: plain text, markdown, or simple JSON only.

## Regression Checklist

After updating, confirm:

1. `SKILL.md` still tells an agent when to use the skill and how to navigate it.
2. No core concept lives in two different reference files with conflicting wording.
3. The scenario playbook still reflects the newest heuristics.
4. `source_index.md` explains which sources informed which ideas.
5. The skill still favors scenario trees, tests, and invalidations over prediction language.
6. `references/assets/` contains a usable offline copy of every source the skill depends on.

## For New Crypto Sources

Specifically check whether the new source adds anything about:

- Bitcoin leadership vs altcoin leadership
- cap-tier rotation
- thematic indexes
- spread-chart usage
- stablecoin / cash refuge behavior
- exogenous shock behavior
- failed signals
- low-liquidity pattern distortions

If yes, update `references/crypto_adaptations.md` and, if the concept is subtle, also `references/uncommon_concepts.md`.

## For New Classical Wyckoff Sources

Specifically check whether the source sharpens:

- phase distinctions
- event definitions
- effort/result reading
- cause/effect and point-and-figure logic
- trade-location hierarchy
- significant bar or trend-control logic

If yes, update `references/book_foundations.md`.

## Preferred Change Style

- Add compact, durable statements.
- Prefer one strong paragraph or a short bullet set over long prose.
- Preserve older archive-derived nuances unless the new source clearly supersedes them.

## Final Step

When the update is complete, add a short dated note to your working changelog outside the skill if you need one, but do not create extra documentation inside the skill unless it directly improves skill use.
