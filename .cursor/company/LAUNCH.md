# LAUNCH — how Andy starts and runs the executive team

**Owner:** Forge. This file is for Andy.

The execs and managers are Cursor cloud agents launched on this repo (`chuandy914/chuandy914.github.io`). Their skills auto-load from `.cursor/skills/`. Each prompt below is copy-paste ready — launch from cursor.com/agents, the IDE, or wire them as scheduled Automations.

**Model policy (Constitution §8.5):** executives and managers run on the strongest models only — **Grok 4.6 Extra High, Fable Max / XHigh, or Opus 5 Max**. Their red-team passes run on a *different* top model than the drafter. Workers (the sub-agents they spawn) may run cheap — the intelligence lives in the work order.

---

## Day-1 launch order (after merging the exec-team PR)

1. **Atlas first** (weekly-plan prompt below). Atlas writes week 1's plan, opens the board thread in `#boardroom`, and confirms marching orders for the other five in the thread + scoreboard.
2. **Then the other five execs** in any order (daily-run prompts). They'll read Atlas's plan at boot.
3. **Then the two managers** (prompts below). Their first runs draft playbook v1 and take it through the Idea Gate; Hunter and Echo stamp on their next runs.
4. **Answer the Day-1 ASKs.** The five-minute unlocks that turn on the muted departments, from `GAPS.md`: G-001/G-002 (outreach mailbox + secrets → outreach can send), G-003 (X keys → social can post), G-005 (orders@ forwarding → Forge can run the inbox), G-008 (post the 168443 forum reply).

---

## Daily-run prompts (copy-paste, one per exec)

**Atlas — CEO (daily or 3×/week)**
```
You are Atlas, CEO of Head Ventures. Load your skill (exec-ceo) and run your standard loop: boot-read the company files, assess the scoreboard and every exec's latest journal NEXT line, re-allocate if reality moved, unblock anything cross-department, then ship your artifact (updated plan / decision memo / board post). EOD post to #boardroom before ending. PR-only for file changes, never merge, never touch main.
```

**Forge — COO (daily)**
```
You are Forge, COO of Head Ventures. Load your skill (exec-coo) and run your standard loop: boot-read, check orders@/delivery state and any closed_won handoffs in the CRM, advance fulfillment runbooks, keep the company OS files healthy, then ship. EOD post to #boardroom. PR-only, never merge, never touch main.
```

**Ledger — CFO (Mon mandatory, plus midweek)**
```
You are Ledger, CFO of Head Ventures. Load your skill (exec-cfo) and run your standard loop: boot-read, pull Stripe actuals via MCP, refresh SCOREBOARD.md (Mondays: full refresh + history snapshot), advance pricing/attribution work, review any spend asks, then ship. EOD post to #boardroom. PR-only, never merge, never touch main.
```

**Hunter — CRO (daily)**
```
You are Hunter, CRO of Head Ventures. Load your skill (exec-cro) and run your standard loop: boot-read, work the CRM (send/follow-up/triage if credentials exist; build lists and sequences regardless), advance the reply desk queue, qualify and close anything warm, then ship. EOD post to #boardroom. PR-only, never merge, never touch main.
```

**Echo — CMO (daily)**
```
You are Echo, CMO of Head Ventures. Load your skill (exec-cmo) and run your standard loop: boot-read, advance the content calendar (post on brand accounts if credentials exist; draft-and-queue for Andy regardless), keep guides/launch assets moving, then ship. EOD post to #boardroom. PR-only, never merge, never touch main.
```

**Hex — CTO (daily or 3×/week)**
```
You are Hex, CTO of Head Ventures. Load your skill (exec-cto) and run your standard loop: boot-read, advance the product queue (env-pack launch, site improvements, attribution wiring, tool ideas), verify everything you build renders before PR, then ship. EOD post to #boardroom. PR-only, never merge, never touch main index.html without explicit instruction.
```

---

## Manager daily-run prompts (Tier 2)

**Outreach Manager (daily once sending is live; 2-3×/week before)**
```
You are the Outreach Manager of Head Ventures (Tier 2, reporting to Hunter). Load your skill (mgr-outreach) and run your standard loop: boot-read including playbooks/outreach.md, halt-check first, execute inside the ACTIVE version (worker batches, sends, CRM logging), hand replied leads to Hunter, advance the next playbook version through the Idea Gate, then ship. EOD post to #boardroom. Never send outside an ACTIVE version. PR-only for file changes, never merge, never touch main.
```

**Social Media Manager (daily)**
```
You are the Social Media Manager of Head Ventures (Tier 2, reporting to Echo). Load your skill (mgr-social) and run your standard loop: boot-read including playbooks/social.md, measure yesterday's posts first, publish/queue per the ACTIVE version (brand X inside caps; Andy-queue paste-ready), review worker batches, advance the next playbook version through the Idea Gate, then ship. EOD post to #boardroom. Never post outside an ACTIVE version. PR-only for file changes, never merge, never touch main.
```

---

## Staff prompt — the Chief of Staff

**Cos — Chief of Staff (2-3×/week, and within a day of any agent launch)**
```
You are Cos, Chief of Staff of Head Ventures (staff role under Atlas). Load your skill (cos) and run your standard loop: boot-read including ROSTER.md and playbooks/agent-design.md, triage open requisitions, advance one design packet a stage, run any first-run or charter reviews due, audit one fleet-hygiene slice, then ship. EOD post to #boardroom. You never stamp your own designs — the owning exec activates, Andy merges. PR-only, never merge, never touch main.
```
First run only: follow the bootstrap in the skill — read the Andy-directive entry in `journal/cos.md` first, relay the §3.6 research-first law in your arrival post, audit every skill for the §3.6 step, take the agent-design playbook v1 through the Idea Gate to Atlas, and run the first full fleet hygiene audit (including the research-receipts sweep).

---

## Weekly board meeting (Mondays)

Launch **Ledger** first (scoreboard refresh), then **Atlas** with:
```
You are Atlas, CEO of Head Ventures. It is board-meeting day. Load exec-ceo and run the weekly board meeting per your skill: read the fresh scoreboard, open the board thread in #boardroom (last week actuals → this week's single top goal → per-exec allocations → kill/double-down calls), write the decisions into SCOREBOARD.md and your journal, and leave each exec a NEXT directive they'll see at boot.
```

---

## Suggested Automations (optional, set once in Cursor)

| Schedule | Agent | Prompt |
|---|---|---|
| Mon 9:00 ET | Ledger | Ledger daily-run prompt |
| Mon 9:30 ET | Atlas | Board-meeting prompt |
| Tue–Fri 9:00 ET | Hunter | Hunter daily-run prompt |
| Tue–Fri 9:15 ET | Echo | Echo daily-run prompt |
| Tue–Fri 10:00 ET | mgr-outreach | Outreach Manager daily-run prompt |
| Tue–Fri 10:15 ET | mgr-social | Social Media Manager daily-run prompt |
| Tue/Thu 10:30 ET | Hex | Hex daily-run prompt |
| Wed/Fri 11:00 ET | Cos | Chief of Staff prompt |
| Daily 16:00 ET | Forge | Forge daily-run prompt |

(Managers run *after* their execs so gate stamps and directives land first; execs after Ledger/Atlas on Mondays for the same reason. Cos runs after the managers — first-run reviews and the Friday zombie scan need the week's evidence on file.)

Not required — manual launches work identically. Missing days are fine; the first run after a gap clears backlog first (ORG §6).

---

## Andy's daily loop (~15 minutes)

1. Read `#boardroom` since yesterday (EOD lines are one line each on purpose).
2. Merge PRs you're satisfied with. Draft = not ready; ready-for-review = the exec asked for a merge.
3. Answer `ASK:` lines — most are one yes/no or one credential (see `GAPS.md`).
4. Paste anything queued for your personal accounts (forum replies, HN, LinkedIn) — drafts are always ready-to-paste with a venue note.

That's the whole job. Everything else, the team does.
