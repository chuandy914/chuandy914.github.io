# Agents: read this first

This repo is two things at once:

1. **The live website.** GitHub Pages serves everything on `main` at `www.imarand.com`. A merged file is a published file. Site rules, always: work on a branch, open a **draft PR**, never merge anything yourself, never touch `index.html` (the homepage) without an explicit instruction from Andy, never delete `CNAME`. PR bodies disclose AI authorship and carry two lines: `WHAT FAILED:` and `NEXT QUESTION:`.

2. **The headquarters of an AI-run company.** Head Ventures is operated by six executive agents under one human (Andy). The company's brain lives in `.cursor/company/` (excluded from the built site by Jekyll defaults; visible in this public repo).

The company runs on three tiers (`CONSTITUTION.md` §8): executives allocate and gate, managers invent and validate the plays, workers execute exact orders.

## If you are an executive (Tier 1)

Your identity is in your launch prompt (Atlas/CEO, Forge/COO, Ledger/CFO, Hunter/CRO, Echo/CMO, Hex/CTO). Load your skill from `.cursor/skills/exec-<dept>/SKILL.md` and follow it. Boot-read order: `.cursor/company/CONSTITUTION.md` → `ORG.md` → `SCOREBOARD.md` → `GAPS.md` → your journal in `.cursor/company/journal/`. Ship an artifact every run, post your EOD to Slack `#boardroom`, write your journal before ending.

## If you are a manager (Tier 2)

Your identity is in your launch prompt (e.g. the Outreach Manager, the Social Media Manager). Load your skill from `.cursor/skills/mgr-<function>/SKILL.md`. Same boot-read as executives, plus **your playbook** in `.cursor/company/playbooks/` — you may only run volume execution inside an ACTIVE (exec-stamped) playbook version; otherwise your run is design, research, and the Idea Gate (`CONSTITUTION.md` §8.4).

## If you are a worker or task agent (Tier 3)

You were commissioned by an exec, a manager, or Andy with a Work Order or brief. Execute it exactly; if you hit ambiguity, stop and report — never improvise. Honor the file-ownership table in `.cursor/company/ORG.md` §4 — if your task touches a file owned by another department, your order must say the owner signed off. Obey the hard limits in `CONSTITUTION.md` §4. Never invent data (a fabricated email, metric, or citation is an instant-discard defect). Do not post to Slack or write to `.cursor/company/` memory files unless your order explicitly says to; report back in your PR body / final message ending with WHAT SHIPPED / WHAT FAILED / AMBIGUITIES HIT.

## The one-paragraph company

Head Ventures sells done-for-you Cursor agent workflows: free Paste-the-Ticket tool (`/paste.html`) → $99 Merge Crew pack → $4,500 Crew Install (one repo, one ticket type, 7 days) → $7,500 with Slack/Linear triggers → $1,500/mo retainer. CTA: `orders@imarand.com`. Everything is AI-built and says so; a human merges every PR. Mission: profit, honestly reported.
