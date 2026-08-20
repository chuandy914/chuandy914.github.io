# ROSTER — every persistent agent, its grade, and its review date

**Owner:** Cos (Chief of Staff). Any exec/manager appends requisition rows (§3); only Cos edits the registry.
**Scope:** persistent agents only (Tiers 1–2 + staff). Workers are never rostered — they are disposable by law (Constitution §8.3).
**Law:** `ORG.md` stays canonical for structure and decision rights; this file is the operational registry — lifecycle states, review dates, and the requisition queue. A roster row that doesn't match reality is a Cos KPI defect.

**Lifecycle states:** `DESIGN` (packet in progress) → `GATED` (red-teamed + exec-stamped, awaiting merge/launch) → `LIVE` → `RETIRED` (archived, never deleted). `HALTED` = launch pulled pending redesign.

---

## 1. The registry

### Tier 1 — Executives (constitutional; no +4-week reviews — ORG §8 departments law applies)

| Agent | Role | Skill | Journal | Status | Graded on |
|---|---|---|---|---|---|
| Atlas | CEO | `.cursor/skills/exec-ceo/` | `journal/ceo.md` | LIVE | Net new revenue/wk, plan hit rate, kill latency |
| Forge | COO | `.cursor/skills/exec-coo/` | `journal/coo.md` | LIVE | Fulfillment SLA, OS-file health |
| Ledger | CFO | `.cursor/skills/exec-cfo/` | `journal/cfo.md` | LIVE | Scoreboard truth, pricing/attribution |
| Hunter | CRO | `.cursor/skills/exec-cro/` | `journal/cro.md` | LIVE | Pipeline, qualified conversations, closes |
| Echo | CMO | `.cursor/skills/exec-cmo/` | `journal/cmo.md` | LIVE | Attention → funnel handoffs |
| Hex | CTO | `.cursor/skills/exec-cto/` | `journal/cto.md` | LIVE | Site/product ships, conversion surfaces |

### Staff (Tier-2 contract, chartered by Atlas)

| Agent | Role | Skill | Journal | Playbook | Chartered | Review due | Status | Graded on |
|---|---|---|---|---|---|---|---|---|
| Cos | Chief of Staff | `.cursor/skills/cos/` | `journal/cos.md` | `playbooks/agent-design.md` | 2026-08-20 (Andy mandate) | 2026-09-17 | GATED — LIVE on merge | Time-to-live ≤3 runs, first-run artifact rate 100%, zombies 0 |

### Tier 2 — Managers

| Agent | Function | Reports to | Skill | Journal | Playbook | Chartered | Review due | Status | Graded on |
|---|---|---|---|---|---|---|---|---|---|
| mgr-outreach | Outreach: the how | Hunter | `.cursor/skills/mgr-outreach/` | `journal/mgr-outreach.md` | `playbooks/outreach.md` | 2026-08-20 | 2026-09-17 | LIVE | Reply rate ≥5%, positive share ≥40%, 0 spam signals |
| mgr-social | Social: the how | Echo | `.cursor/skills/mgr-social/` | `journal/mgr-social.md` | `playbooks/social.md` | 2026-08-20 | 2026-09-17 | LIVE | Engagement, funnel handoffs, cap compliance |

---

## 2. Review calendar (Cos maintains; next due first)

| Date | Review | Owner of verdict |
|---|---|---|
| within 1 Cos run of launch | First-run review — every newly launched agent (playbook §8) | Cos |
| 2026-09-17 | Charter review: mgr-outreach | Hunter (Cos prepares) |
| 2026-09-17 | Charter review: mgr-social | Echo (Cos prepares) |
| 2026-09-17 | Charter review: Cos | Atlas |
| weekly (Fri) | Zombie scan + one hygiene-audit slice | Cos |

---

## 3. Requisitions — ask for an agent here

Append a row; Cos triages within two of its runs (playbook §10). Verdicts are announced in `#boardroom`. A decline usually ships with a consolation artifact (the skill or work-order skeleton that covers the need without headcount).
Status: `open` → `triaged` → `in-design (packet stage)` / `declined (verdict written)` / `launched`.

| ID | From | Function / position | Outcome it would own | Evidence of recurring volume | Status | Opened |
|---|---|---|---|---|---|---|
| — | — | *(example: "inbox triage manager")* | *(one sentence, playbook §2.1)* | *(real counts from journals/scoreboard)* | — | — |

---

## 4. Log — the workforce's provisioning history (append-only)

| Date | Event |
|---|---|
| 2026-08-20 | Founding: six executives + mgr-outreach (Hunter) + mgr-social (Echo) chartered in the company-OS PR. |
| 2026-08-20 | Cos (Chief of Staff, staff role under Atlas) designed and chartered by Andy's direct mandate; agent-design playbook v1 drafted, gate pending Atlas (Cos run 1). |
