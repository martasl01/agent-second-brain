# Craft — Writing Techniques

The rules of the craft: how a post is built before it's tuned for a platform. Load this for drafting, structural rewrites, and editing passes. Platform-specific overrides live in `platforms/`.

> **Provenance:** This is a *content second brain* modeled on the architecture in Pawel Huryn's case study ("From 4 hours to 30 minutes a day"). Rules marked **[from case study]** are the patterns the article reports with data. Everything else is a **starter** — a sensible default seeded at setup, to be confirmed or killed by your own data. Do not treat starters as proven.

---

## Rules

### Rule 1 — Data experiments beat opinion **[from case study]**
A post that runs a small experiment and shows the result earns roughly **3× the bookmarks** of an opinion/take post.
*Implication:* when an idea can be framed as "I tried X, here's what happened," prefer that framing over "here's what I think about X."
*Evidence:* reported in the case study (graduated from HYP — see `hypotheses/index.md` HYP-002).

### Rule 2 — Builder-teacher voice outperforms the analyst take **[from case study]**
Posts written as a builder *teaching* what they did consistently beat posts written as an analyst *commenting* on a topic.
*Implication:* default to `voice/archetypes.md` → **Builder-Teacher**. Reach for Analyst only when the post is explicitly a synthesis/landscape piece.
*Evidence:* reported in the case study (graduated — see HYP-003).

### Rule 3 — One post, one idea (starter)
A post carries exactly one claim the reader can repeat in a sentence. Second ideas become second posts.
*Test signal:* if you can't write the one-line takeaway before drafting, the post isn't ready.

### Rule 4 — Show the work, not just the conclusion (starter)
Specifics (numbers, before/after, the exact thing you changed) earn saves; abstractions get scrolled past. Replace adjectives with evidence.

---

## Post anatomy (default skeleton)

1. **Hook** — line 1 earns line 2. Platform rules in `platforms/`. Lead with tension, a number, or a negation, not a throat-clear.
2. **Promise / stakes** — why this is worth the reader's next 20 seconds.
3. **Body** — the work: steps, the experiment, the before/after. One idea (Rule 3).
4. **Takeaway** — the one line they'll repeat or bookmark.
5. **(Optional) invitation** — a question or a "reply if…" only when it's genuine, not engagement-bait.

---

## The editing loop (10+ iterations) **[from case study]**

The case study frames quality as **10+ iterations per post**, not "write me a post about X." The human makes every editorial call (what to post, what to kill, the angle); the agent supplies research, verification, structural variants, and pattern-matching against this knowledge base.

Per pass, the agent should be able to do one of:
- propose 2–3 alternative hooks (and say which it expects to win and why, citing a rule),
- tighten — cut throat-clearing, hedges, and any sentence that doesn't carry the one idea,
- fact-check load-bearing claims against primary sources before they ship,
- flag where the draft relies on a **hypothesis** (not a rule) per the Hard Constraints in `CLAUDE.md`.

---

## The data-experiment format (high-value template)

Because of Rule 1, this is the workhorse structure:

```
Hook:      [the question or the surprising result, stated as a number or negation]
Setup:     [what I tried, in one line — the smallest version of the experiment]
Result:    [what actually happened — the number, the before/after]
Why:       [the one-sentence mechanism — why it happened]
Takeaway:  [what the reader should now do differently]
```

Keep the setup small enough that the reader believes they could run it too.

---

## Anti-patterns (avoid)

- **Positive-platitude hooks** — see `platforms/linkedin.md` Rule 1; negation outperforms on LinkedIn.
- **Two ideas in one post** — violates Rule 3; split it.
- **Conclusion without the work** — violates Rule 4; readers don't save assertions.
- **Engagement-bait questions** — erode trust faster than they earn replies.
