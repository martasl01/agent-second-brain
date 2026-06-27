# Hypothesis Index — Content

This is the system's learning layer. Hypotheses are things you're testing — not yet rules, but not random guesses either. They should be specific enough to confirm or deny. Data points come from `../posts/performance-log.md`.

> **Provenance:** HYP-001/002/003 are the three findings the **case study reports with data**, so they're logged here as *graduated* (their rules now live in the craft files). Their evidence summary cites the case study rather than your own per-post log — re-confirm against your audience as you accumulate real posts. HYP-004+ are **starter active hypotheses**: falsifiable defaults with no evidence yet.

---

## How This Works

**Hypothesis → Rule** (graduation): 3+ supporting data points, 0 strong counter-examples → graduate. Move the insight to the relevant craft file as a rule.
**Hypothesis → Rejected**: 2+ data points against, or 0 support after 8+ tests → reject. Move to `rejected.md`.
**Active**: being tested; don't enforce as a rule yet. **On hold**: paused, no active way to test.

Full graduation/rejection criteria and the schema live in `EXAMPLE.md` and in `../../system-maintenance.md`.

---

## Active Hypotheses

### HYP-004
**Statement:** On X, a single-tweet data experiment earns more bookmarks than a thread covering the same idea.
**Status:** active
**Created:** 2026-06-27
**Context:** X (Twitter), builder-teacher / experimenter voice.
**Evidence for:**
- [none yet]
**Evidence against:**
- [none yet]
**Notes:** Test by posting matched pairs (same idea, two formats) and comparing bookmarks. Starter hypothesis.

### HYP-005
**Statement:** Negation hooks beat positive hooks on **X** too (generalization of the LinkedIn finding, HYP-001).
**Status:** active
**Created:** 2026-06-27
**Context:** X (Twitter), any voice.
**Evidence for:**
- [none yet]
**Evidence against:**
- [none yet]
**Notes:** If confirmed with 3+ points incl. one outside the original LinkedIn context, graduate into `../platforms/x-twitter.md`. Starter hypothesis.

### HYP-006
**Statement:** Posts in the "knowledge systems / second brains" lane (topic lane 4) earn above-median bookmarks for this account.
**Status:** active
**Created:** 2026-06-27
**Context:** Both platforms; lane defined in `../topic-lanes.md`.
**Evidence for:**
- [none yet]
**Evidence against:**
- [none yet]
**Notes:** If true, raise that lane's drafting priority. Starter hypothesis.

---

## Graduated Hypotheses

*(One-line stubs for traceability. Full rule lives in the target craft file.)*

### HYP-001
**Statement:** On LinkedIn, negation hooks outperform positive hooks.
**Status:** graduated
**Graduated:** 2026-06-27
**Now lives in:** `../platforms/linkedin.md` as Rule 1
**Evidence summary:** Reported in the case study. Re-confirm against own data via `../posts/performance-log.md`.

### HYP-002
**Statement:** Data-experiment posts earn ~3× the bookmarks of opinion/take posts.
**Status:** graduated
**Graduated:** 2026-06-27
**Now lives in:** `../writing-techniques.md` as Rule 1
**Evidence summary:** Reported in the case study (≈3× bookmarks). Re-confirm against own data.

### HYP-003
**Statement:** Builder-teacher posts outperform analyst takes.
**Status:** graduated
**Graduated:** 2026-06-27
**Now lives in:** `../writing-techniques.md` as Rule 2 (and default voice in `../voice/archetypes.md`)
**Evidence summary:** Reported in the case study. Re-confirm against own data.

---

## Rejected Hypotheses

*(Stubs only — full entries with killing evidence live in `rejected.md`.)*

- *(none yet — see `rejected.md` for the immune-memory format and the one illustrative starter.)*

---

## Schema Reference

See `EXAMPLE.md` for a fully-worked example at each lifecycle stage. When adding a hypothesis:

```markdown
### HYP-[NEXT NUMBER]
**Statement:** [Precise, falsifiable claim with a measurable signal.]
**Status:** active
**Created:** [DATE]
**Context:** [Where/when this applies]
**Evidence for:**
- [none yet]
**Evidence against:**
- [none yet]
**Notes:** [How you'll test this]
```

Good hypotheses are falsifiable, specific (claim + context + measurable signal), and distinct from existing rules.
