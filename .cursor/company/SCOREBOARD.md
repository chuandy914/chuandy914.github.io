# Head Ventures — Company Scoreboard

**Owner:** Ledger (CFO). Refreshed every Monday from Stripe actuals before the board meeting; deltas allowed any run.
**Rule:** real numbers only. `unknown` is a valid value; an invented value is a firing offense (Constitution §2.6). Estimates are labeled `est.` and never appear in public claims.

---

## Week of 2026-08-17 → 2026-08-23 (seed week — first Ledger run must replace every `unknown` with Stripe actuals or an explicit zero)

### Money (Stripe actuals — Ledger)
| Metric | This week | Prior week | Notes |
|---|---|---|---|
| Net new revenue | unknown | unknown | Pull from Stripe MCP: charges + payment-link sessions |
| $99 packs sold | unknown | unknown | |
| $49 env-packs sold | 0 | 0 | Product unlaunched — Hex owns launch |
| Installs paid ($4,500/$7,500) | unknown | unknown | |
| Retainers active ($1,500/mo) | unknown | unknown | |
| Refunds | unknown | unknown | |

### Pipeline (Hunter)
| Metric | This week | Prior week | Notes |
|---|---|---|---|
| Leads added to CRM | 0 | — | CRM created 2026-08-20, empty |
| Cold emails sent | 0 | — | Blocked on G-001/G-002 (mailbox + creds) |
| Replies received | 0 | — | |
| Qualified conversations (repo or ticket type exchanged) | 0 | — | The install metric that matters |
| Deals closed | 0 | — | |

### Attention (Echo)
| Metric | This week | Prior week | Notes |
|---|---|---|---|
| Posts published (brand accounts) | 0 | — | Blocked on G-003 (X account+keys) |
| Drafts queued for Andy's personal accounts | 0 | — | |
| Guides live | 2 | 2 | issues-scope, env-setup-400 |
| Launches | 0 | — | Show HN drafted in memo (PR #7 appendix), not posted |

### Machine (Hex) & Delivery (Forge)
| Metric | This week | Prior week | Notes |
|---|---|---|---|
| Site PRs opened / merged | 3 open (#6 #7 #8) / 0 | — | |
| Experiments running (attribution surfaces) | 0 | — | Per-surface payment links not yet created |
| Orders fulfilled / SLA misses | unknown / unknown | — | Forge needs orders@ visibility (G-005) |

---

## How Ledger refreshes this file (runbook pointer)
Full runbook in `.cursor/skills/exec-cfo/SKILL.md`. Short form: `get_balance_summary` + `stripe_api_read` (charges, checkout sessions, payment links) for the trailing 7 days → fill Money table → pull Pipeline row counts from `crm/pipeline.csv` → pull Attention/Machine counts from calendar + GitHub → commit with message `scoreboard: week of <date>` → post the Money+Pipeline summary lines to #boardroom.

## History
*(Ledger appends a dated snapshot section here each Monday before overwriting the current-week tables. Never delete history.)*
