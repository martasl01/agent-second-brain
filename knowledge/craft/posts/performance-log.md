# Posts — Performance Log

The feedback layer. Every analyzed post gets logged here with its metrics and the patterns it confirms or challenges. This is where rules earn their evidence and hypotheses get their data points. In the case study, this is the data that let the system "notice patterns I missed."

> **Provenance:** The *one seeded entry* below restates a finding the case study reports (data-experiment > opinion on bookmarks). It is logged as a reference data point, not a real post of yours. **Replace and extend with your actual posts** — pull metrics from X/LinkedIn analytics (the case study built a small script for this).

---

## How to log a post

Add an entry per analyzed post. Keep it scannable — this file is read during drafting to recall what's worked.

```
### [DATE] — [platform] — [one-line topic]
**Voice:** [archetype from ../voice/archetypes.md]
**Lane:** [from ../topic-lanes.md]
**Format:** [data-experiment | builder-teacher | thread | take | other]
**Metrics:** [impressions / likes / bookmarks / engagement %]
**Hook:** [the actual first line]
**Confirms / challenges:** [which rule or HYP-ID this is a data point for]
**Note:** [what to repeat or avoid next time]
```

### Metrics that matter (priority order)
1. **Bookmarks** — strongest "worth returning to" signal (especially on X).
2. **Engagement rate** — normalizes for reach.
3. Reposts/shares — distribution.
4. Likes — weakest signal; cheap.

---

## Entries

### [reference] — X — data-experiment vs. opinion **[from case study]**
**Format:** data-experiment vs. take (comparison)
**Metrics:** data-experiment posts ≈ **3× bookmarks** of opinion posts
**Confirms:** `../writing-techniques.md` Rule 1 / HYP-002 (graduated)
**Note:** seeded from the case study as a reference data point — not one of your posts. Log your own to confirm it holds for your audience.

*(Add your real posts below. Each one is a data point that can graduate a hypothesis or challenge a rule.)*

---

## How this feeds the learning loop

- A pattern that shows up across **3+ posts** with no strong counter-example → graduate the hypothesis to a rule (see `../hypotheses/index.md`).
- A post that **contradicts** an existing rule → don't edit the rule; open a hypothesis with the counter-evidence (Hard Constraints in `CLAUDE.md`).
- A belief that posts keep disproving → move it to `../hypotheses/rejected.md` so you stop re-testing it.
