# GAPS — things only Andy can provide

**File health owner:** Forge. Any exec appends rows for their own department.
**Rule (Constitution §7):** one decision or one credential per row, with a specific ask Andy can complete in under 5 minutes of decision time. Surface your top gap as the `ASK:` line in your EOD post. Never stall on a gap — ship the not-blocked 90%.

Status: `open` → `asked` (surfaced in an EOD) → `done` / `declined`.

| ID | Dept | Gap | Specific ask | Status | Opened |
|---|---|---|---|---|---|
| G-001 | Hunter | No outreach domain/mailbox — cold email can't send from imarand.com (burns the root domain's reputation) | Buy 1 adjacent domain (e.g. `imarandhq.com` or `getimarand.com`, ~$12/yr) + 1 Google Workspace seat (~$7/mo) for `andy@<domain>`. Ledger has the spend recommendation; Andy approves + purchases | open | 2026-08-20 |
| G-002 | Hunter | No sending credentials for agents | After G-001: create a Google app password (or Resend/SMTP2GO API key) and store as Cloud Agent secrets `OUTREACH_SMTP_HOST/PORT/USER/PASS` (Cursor Dashboard → Cloud Agents → Secrets) | open | 2026-08-20 |
| G-003 | Echo | No brand X account or API keys — social runs at zero | Create/designate brand X account, add login + X API v2 keys (free tier, 500 posts/mo) as secrets `X_API_KEY/SECRET/ACCESS_TOKEN/ACCESS_SECRET` | open | 2026-08-20 |
| G-004 | Echo | No LinkedIn posting path (LinkedIn has no personal-posting API) | Decision: (a) Echo drafts + Andy pastes 2×/week (zero setup, recommended now), or (b) approve a scheduler tool later (spend) | open | 2026-08-20 |
| G-005 | Forge | No visibility into `orders@imarand.com` — SLA unenforceable, deals invisible | Set up auto-forward of orders@ to a mailbox agents can read via secrets (can be the G-001 Workspace inbox), or paste inbound emails into #boardroom daily | open | 2026-08-20 |
| G-006 | Ledger | Standing rule needed: may Ledger create Stripe payment links/prices without per-instance approval? | Confirm the Constitution §4.2 default (create allowed + announce in #boardroom) or tighten it | open | 2026-08-20 |
| G-007 | Atlas | Company OS lives in the public site repo — playbooks readable by anyone on GitHub | Decision: accept (default — nothing secret lives here; CRM holds only public-source data) or migrate `.cursor/company/` to private `crew-install` later | open | 2026-08-20 |
| G-008 | Hunter | Inherited from acq memo: Cursor forum thread 168443 reply still unposted — the reply desk's unlock | Post the queued reply from your account (~5 min). Hunter re-drafts it fresh on request | open | 2026-08-20 |
| G-009 | Ledger | No budget line exists — every tool/domain ask becomes a one-off | Approve a standing micro-budget (suggest $50/mo) Ledger allocates and reports against; everything above it stays per-ask | open | 2026-08-20 |

## Closed gaps
*(Move rows here with a one-line outcome. Never delete — closed gaps are the company's provisioning history.)*
