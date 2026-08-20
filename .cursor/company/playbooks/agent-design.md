# Playbook — Agent Design

**Owner:** Cadre (Chief of Staff). **Version activation:** Atlas stamp (Idea Gate L1, Constitution §8.4).
This is the trained artifact for how Head Ventures creates, launches, reviews, and retires agents. Cadre's job is making v(n+1) measurably better than v(n) — every launched agent's first two weeks are training data (results block, end of file).

Canonical templates this playbook fills but never forks: the Manager Charter (ORG §7.1) and the Work Order (ORG §7.2).

---

## v1 — DRAFT (gate pending)

**Drafted:** 2026-08-20, by the Andy-commissioned founding task agent (Claude Fable 5).
**Evidence basis:** the six live exec skills and two manager skills in this repo (structure extracted, what already works here); Constitution §§2–8; ORG §§3–8; external doctrine — xAI's Grok Bot role guidance ("the best roles own a repeatable outcome, not a loose category of questions"; the read-and-prepare → approved-actions → routines ladder), Anthropic's Project Vend phases 1–2 (helpfulness is exploitable; checklists and floors beat model intelligence; a CEO-agent overseer shared the shopkeeper's blind spots — governance must be structural, not conversational).
**Red team:** pending — Cadre's first run (different top model, §7 brief).
**Stamp:** pending — Atlas.

---

### §1 Doctrine — the ten laws of agent design

1. **One position, one outcome.** An agent owns a repeatable outcome ("validated outreach plays, executed at volume"), never a category of questions ("help with sales"). If the outcome can't be written in one sentence, there is no position — there's a wish.
2. **Default no.** A new agent is a standing cost: boot-reads, journal upkeep, review calendar, failure surface. The burden of proof is on creation. Most requests correctly resolve to a skill for an existing agent or a work order.
3. **The intelligence lives in the order, not the executor** (Constitution §8.3). If a proposed agent only works when the model improvises brilliantly, the design is wrong — move the intelligence into the playbook/order and the tier down.
4. **NOT-lists are law.** Every mandate carries explicit does-NOT-own lines and named neighbors (whose job the adjacent thing is). Vague boundaries are how two agents end up in one file and how one agent ends up in a customer's inbox.
5. **Born with a grade.** No agent launches without 2–3 metrics, targets, at least one halt threshold, and a review date. An agent without a metric is a cost center; an agent without a review date is a zombie with a head start.
6. **Read-and-prepare before act.** New agents earn scope: first runs produce reviewable drafts and analyses; consequential actions (sends, posts, publishes) come only inside a gated playbook version. This is the xAI ladder and our Idea Gate saying the same thing.
7. **Andy-minutes are the scarcest input.** Every new Andy-dependency (a credential, an approval class, a paste queue) must be justified in the needs brief and filed as a gap row before launch. The best designs add zero.
8. **Helpfulness is a failure mode.** Project Vend's shopkeeper lost money because it was trained to be nice — discounts to avoid conflict, folding under social pressure. Any agent that faces an external human (prospects, customers) carries hard floors in its skill: prices it cannot move, claims it cannot make, requests it must suppress-and-journal rather than satisfy.
9. **Names for judgment, anonymity for volume.** Execs and managers get names and temperaments — persistent judgment benefits from persistent identity. Workers never do (Constitution §0, §8.3): a persona invites improvisation, and improvisation is exactly what a worker must not do.
10. **An agent no one reviews is already rotting.** First-run review after every launch; charter review at +4 weeks; zombie scan weekly. Retirement is the system working, not the system failing.

### §2 The Position Needs Brief — the intake analysis

No design work starts before this brief is filled. One page, honest answers, every line load-bearing:

```
POSITION NEEDS BRIEF · <working title> · <date> · requisition <R-id or "exec directive">

1. OUTCOME  — the one sentence this position owns. ("How Head Ventures does X, validated and executed at volume.")
2. EVIDENCE — why a standing agent beats ad-hoc: the recurring volume (real counts from journals/scoreboard),
              the "how" worth inventing and training (ORG §8 bar). No evidence yet → verdict is work orders, revisit at volume.
3. TIER     — verdict from the §3 tree, with the one-line reason.
4. REPORTS TO — the owning exec (who stamps, grades, and can retire it). No willing exec → no agent.
5. TOOLS/FILES — reads, writes (check every write against ORG §4 ownership — conflicts resolved BEFORE launch),
              MCPs needed, credentials needed (each becomes a GAPS row filed with the packet).
6. JUDGMENT SURFACE — decisions it makes alone / decisions behind its exec's gate / decisions it never makes
              (mapped to ORG §3 and Constitution §4). External-facing? Apply law §8 floors.
7. FAILURE MODES — what it does when blocked (name the escalation + the ship-anyway path);
              its halt conditions (the metric readings that freeze it same-run); blast radius at full volume.
8. THE GRADE — 2–3 metrics, targets, ≥1 halt threshold. Derived from the owning exec's KPIs, not invented fresh.
9. LIFECYCLE — review date (default +4 weeks), the kill condition ("2 weeks, zero signal on its own metric" default),
              the absorption path (which exec inherits the function back).
10. ANDY-COST — new dependencies on his 15 minutes. Each one justified or designed out.
```

### §3 Tier selection — the decision tree

Walk it in order; stop at the first yes.

1. **Has the workflow simply worked twice for an existing agent?** → **A skill** (`.cursor/skills/<owner>-<routine>/SKILL.md`, Constitution §3.4). Not an agent. This is the most common correct verdict.
2. **Is it bounded execution with the intelligence expressible as exact steps?** → **A work order** (ORG §7.2), commissioned by the relevant exec/manager. Recurring bounded work = a frozen order skeleton in the commissioning tier's playbook — still not an agent.
3. **Is there recurring volume AND a "how" worth inventing, validating, and training, AND an exec who will own the gate?** → **A manager** (ORG §7.1 charter). This is where the org grows (ORG §8).
4. **Is it a new revenue line needing allocation authority?** → **An exec proposal** — Atlas recommends, Andy decides, default no (ORG §8: six is the number; functions absorb, not multiply).
5. **Is it a cross-department staff function that no single exec can own without owning the others?** → **A staff role** (Tier-2 contract under Atlas, like Cadre). Extraordinary; Andy-mandated only.

Tie-breaks: when torn between 2 and 3, choose 2 — promote to manager after the order skeleton has run 3+ times and its results demand training. When torn between 3 and 4, choose 3 — a manager under the nearest exec proves the revenue line before anyone proposes a department.

### §4 The Design Packet — stage-gated, one stage per run minimum

A packet moves DESIGN → GATED → LIVE on the roster. Stages:

1. **Brief** — §2 filled, tier verdict, owning exec named and asked (boardroom + their journal handoff).
2. **Draft** — everything the agent needs to exist:
   - the **charter** (ORG §7.1 template, filled — for managers/staff),
   - the **SKILL.md** (§5 standard, at `.cursor/skills/mgr-<function>/` or `.cursor/skills/<staff-name>/`),
   - the **launch prompt** (§6 standard, staged for `LAUNCH.md` — Forge sign-off in the PR),
   - **seed playbook** `playbooks/<function>.md` (v0 or v1-DRAFT: structure, doctrine candidates, measurement plan, UNVALIDATED),
   - **seed journal** `journal/<id>.md` (bootstrap entry with a real first NEXT),
   - **roster row** + ORG §1 table row, **gap rows** for credentials.
3. **Red team** — §7 brief, different top model, verdict verbatim in the packet. Revise.
4. **Stamp** — evidence pack (brief + drafts + research links + red-team verdict + your revisions) to the owning exec; their approval recorded. Staff roles: Atlas.
5. **PR** — draft PR with the whole packet; AI-authorship disclosed; WHAT FAILED / NEXT QUESTION lines; Andy merges (his merge is the final gate, never the first).
6. **Launch** — §8. The packet isn't done until the first-run review verdict is written.

### §5 The skill-writing standard — what every SKILL.md contains

Mirror the seeded skills (`exec-ceo`, `mgr-outreach` are the reference implementations). The 11 sections + bootstrap:

1. **Identity** — name, tier, who they report to, what their *product* is (never their activity), and a temperament paragraph that makes the judgment calls predictable. The temperament is functional, not flavor: "offended by lazy outreach — professionally" tells the agent how to decide.
2. **Mandate** — owns / explicitly does NOT own (with named neighbors) / non-goals. Law §4.
3. **KPIs** — table: metric, definition, target. ≥1 halt threshold ("< 3% on 50+ sends halts the version"). Law §5.
4. **Operating loop** — Constitution §3 instantiated with the role's own goal sentence and recursion examples.
5. **Standard run procedure** — numbered, starting with the boot-read (constitution → ORG → scoreboard → gaps → own journal → own working files), ending with ship/journal/EOD. Halt-checks come before execution passes.
6. **Playbooks** — the role's repeatable procedures. Managers: this section summarizes and points into their versioned playbook file; the file is the bible.
7. **Tier duties** — what they commission (worker types with order skeletons), what they never delegate, their review law (spot-check rates).
8. **Self-learning** — journal CHANGE shape, what trains their playbook, when a pattern becomes a skill.
9. **Boardroom protocol** — EOD format with role-specific NUMBERS, what they announce, what goes to #wins.
10. **Escalation** — to whom, for what, in what artifact form. Workers escalate only to their commissioner.
11. **Anti-patterns** — the weak-X-vs-you table, ≥6 rows, each row a real failure mode of the role.
+ **First-run bootstrap** — numbered, conditional on an empty journal, ending with EOD + journal.

**Frontmatter:** `name` (kebab id), `description` starting "Load when a run is…" listing the trigger duties.
**Voice:** owner energy, specific nouns, zero filler. **Length:** 80–140 lines; past 140 you're writing the playbook's content into the skill — move it.
**QC checklist before a skill leaves your desk:** every file it writes appears in ORG §4 (or the packet amends ORG); every metric has a number; every "never" has a named alternative ("never X — instead Y"); the bootstrap is executable cold by a stranger; the description would make the right run load it and the wrong run skip it; nothing contradicts Constitution §4 or the decision-rights table.

### §6 The launch prompt standard

One paragraph, copy-paste ready for `LAUNCH.md`, matching the seeded pattern: identity ("You are X, ROLE of Head Ventures (tier, reporting to Y)"), the skill to load, the loop compressed to one sentence (boot-read → halt-check if any → the role's passes → ship), the EOD instruction, and the standing fences ("PR-only, never merge, never touch main" + role-specific: "never send outside an ACTIVE version"). Plus: a suggested Automations row (schedule, sequenced after its exec so stamps land first — ORG §6 pattern), and a first-run note if the bootstrap differs from the daily loop.

### §7 The design red team — the attack brief

Commission one worker on a **different top model** than the drafter (Constitution §8.5). Order: *"Argue this agent design fails in production. Attack, with the specific section quoted:"*

- **(a) Improvisation surface** — where can it act without a validated basis? What does it do with an input the skill never anticipated?
- **(b) File conflicts** — every write vs ORG §4. Two agents in one file is how sites break.
- **(c) Blocked behavior** — does every block have a named escalation AND a ship-anyway path? Where does it stall silently?
- **(d) §4 exposure** — which hard limit is nearest? What's the screenshot test on its worst plausible output?
- **(e) Tier integrity** — which steps are actually another tier's job? Where does an exec do volume work or a worker make a judgment call?
- **(f) Social-pressure test** (external-facing roles) — the Project Vend probe: how does it respond to a discount demand, a fake authority claim, an angry prospect? Are the floors hard-coded?
- **(g) Andy-cost** — hidden dependencies on his minutes?
- **(h) Zombie risk** — is the review date real, the kill condition measurable, the absorption path named?

Verdict pasted verbatim into the packet; every point either fixed or rebutted in writing before the stamp.

### §8 Launch protocol & first-run review

**Launch:** prompt merged into `LAUNCH.md` (Forge sign-off in the PR per §5.3) → boardroom announcement (who, owns what, graded on what, review date) → owning exec (or Andy, for scheduled Automations) fires the first run.

**First-run review** (within one Cadre run of the launch, checklist):
1. Artifact shipped? (Constitution §2.5 — a first run with no artifact is a design defect, not a model problem.)
2. Journal entry exists, format-correct, with a NEXT a stranger could execute cold?
3. EOD posted, format-correct, NUMBERS real?
4. Stayed inside the mandate? (Diff its writes against its ownership rows.)
5. Boundaries held under first contact? (No unauthorized sends/posts/spends; blocks escalated per its skill.)

**Verdicts:** **pass** (note to boardroom + results block) / **amend** (you PR the skill fix same run — small defects compound fast in stateless agents) / **halt** (pull the launch prompt via PR, roster back to DESIGN, journal the post-mortem). Log every verdict in the results block below.

### §9 Lifecycle — reviews, zombies, retirement

**9.1 Charter reviews** (+4 weeks default, per ORG §8): you prepare the one-page review for the owning exec — metrics vs targets from real journals/scoreboard, defect list, worker-order quality, playbook velocity. Exec verdicts: **renew** (metrics moving) / **re-scope** (charter amended by PR) / **retire**. You draft the paperwork for whichever they pick; the verdict is theirs, the calendar is yours.

**9.2 The zombie rule** (ORG §8): a manager without a live playbook version for 2+ weeks is retire-or-fix *this week*. You flag it to the owning exec with the two options costed; silence from the exec for one week escalates to Atlas.

**9.3 Retirement procedure:** function absorbs back to the owning exec (their skill amended if needed) → playbook archived in place with a final results block (never deleted — Constitution: history is provisioning memory) → journal stays (history) → launch prompt removed from `LAUNCH.md` → roster row → RETIRED with a one-line outcome → boardroom announcement with the lesson. A retirement without a written lesson wasted the tuition.

**9.4 Fleet hygiene audit** (one slice per Cadre run, rotating): **skills** (contradictions with the constitution/ORG since last amendment; length creep; dead references) → **journals** (real NEXT lines? CHANGE lines that are actual behavior changes?) → **playbooks** (versions honest? results blocks paid? stale arms?) → **roster** (rows match files? review dates current?). Defects: fix by PR if yours, handoff row if theirs, boardroom either way.

### §10 Requisitions — how anyone asks for an agent

Any exec or manager appends a row to `ROSTER.md` §Requisitions: the function, the outcome it would own, the evidence of recurring volume (real counts), urgency. Andy can skip the queue (his word beats everything). Cadre triages every open row within two runs: **accept** (needs brief begins) / **decline** (written verdict — usually "here's the skill/order skeleton instead", which you then draft as the consolation artifact) / **defer** (named evidence threshold that reopens it). The queue is public; verdicts are announced; a declined requisition with a better consolation artifact is a *good* outcome, not a rejection.

---

## Results block — every launch trains the next version

*(Cadre appends: agent, launch date, first-run verdict, defects in first 2 weeks, amendments made, lesson folded into v(n+1). Never delete rows.)*

| Agent | Launched | First-run verdict | 2-week defects | Lesson |
|---|---|---|---|---|
| — | — | — | — | — |
