---
name: wyckoff-trader-skill
description: Use this skill when building, reviewing, or updating Wyckoff-based market scenarios, especially for crypto assets. It helps map market cycle context, accumulation/distribution structures, phase and event evidence, intermarket dependencies, crypto sector rotation, relative strength, and actionable scenario trees with triggers, invalidations, and campaign logic.
---

# Wyckoff Trader Skill

## Overview

Use this skill to turn raw chart observations into disciplined Wyckoff scenarios. It is optimized for crypto, but the core workflow remains classical Wyckoff: determine context first, identify the active campaign, evaluate phase and event evidence, then express the result as a scenario tree instead of a single prediction.

## When To Use It

Use this skill when the task involves any of the following:

- Building a Wyckoff scenario for Bitcoin, altcoins, sector indexes, or spread charts.
- Deciding whether a structure is accumulation, reaccumulation, distribution, or redistribution.
- Interpreting springs, upthrusts, SOS/SOW, LPS/LPSY, BUEC/FTI, tests, or failed signals.
- Comparing Bitcoin leadership vs altcoin rotation, sector rotation, or risk-on/risk-off behavior.
- Producing a trade or no-trade thesis with trigger, invalidation, and path dependency.
- Updating the skill from new books, reports, blog posts, or market studies.

## Core Rules

- Label last. Start with price/volume behavior, then add structure labels only after the story is coherent.
- Context outranks pattern. A spring in the wrong background is noise.
- Treat all reads as scenarios, not certainties.
- Prefer the path of least resistance, not the most dramatic narrative.
- In crypto, always check intermarket context and internal rotation before committing to a directional view.
- If the evidence is mixed, produce a no-trade or wait scenario instead of forcing a thesis.
- Prefer the bundled local corpus in `references/assets/` over external URLs.

## Workflow

### 0. Prefer Local Corpus

- Start with [assets/index.md](references/assets/index.md).
- Use the local bundled assets before browsing or re-fetching any source.
- For classical Wyckoff source text, use `references/assets/book/`.
- For the crypto archive source text, use `references/assets/crypto_archive/`.

### 1. Build Context First

- Determine the dominant market cycle position on the relevant higher timeframe.
- Note whether the asset is in a buying position, selling position, or neutral position.
- Check whether the range is likely purposeful or just random balance.
- Load [book_foundations.md](references/book_foundations.md) if the structural read is unclear.

### 2. Map The Structure

- Identify the range boundaries, key bars, and path-of-least-resistance clues.
- Decide whether the structure is accumulation, reaccumulation, distribution, or redistribution.
- Evaluate Phase A-E evidence and event sequence.
- For uncertainty around Phase C or Phase D, read [uncommon_concepts.md](references/uncommon_concepts.md).

### 3. Apply Crypto Overlays

- Check S&P, Nasdaq, dollar, or other relevant intermarket gates when the setup depends on macro risk appetite.
- Check Bitcoin leadership vs large caps, mid caps, low caps, and thematic groups.
- Use spread charts for leadership detection, then switch back to tradable USD or perp charts for execution logic.
- Read [crypto_adaptations.md](references/crypto_adaptations.md) for crypto-specific behavior.

### 4. Build The Scenario Tree

- Write the leading scenario.
- Write at least one credible alternate scenario.
- For each scenario, define:
  - structural thesis
  - trigger
  - invalidation
  - expected path
  - intermarket dependency
  - evidence quality
- Use [scenario_playbook.md](references/scenario_playbook.md) for the output contract.

### 5. Express Campaign Logic

- Distinguish between Phase C, Phase D, and Phase E opportunities.
- Note whether the opportunity is an aggressive end-of-range entry, a confirmation entry, or a continuation entry.
- Prefer action -> test -> confirmation logic over premature breakout chasing.
- Treat failed signals as fresh information, not as nuisances.

## Output Contract

Unless the user asks for another format, structure the final scenario with:

1. Context
2. Wyckoff story
3. Phase and event evidence
4. Crypto-specific overlays
5. Leading scenario
6. Alternate scenario(s)
7. Trigger, invalidation, target path
8. What would change the read
9. Trade / wait / no-trade conclusion

## References

- [source_index.md](references/source_index.md): what sources informed the skill and why they matter.
- [assets/index.md](references/assets/index.md): bundled offline corpus of the book and crypto archive.
- [book_foundations.md](references/book_foundations.md): formal Wyckoff framework from the book.
- [crypto_adaptations.md](references/crypto_adaptations.md): crypto-specific behaviors extracted from the archive.
- [uncommon_concepts.md](references/uncommon_concepts.md): high-signal, non-obvious ideas and terminology.
- [scenario_playbook.md](references/scenario_playbook.md): scenario-building checklist and template.
- [skill-updator.md](skill-updator.md): process for updating the skill with new material.
