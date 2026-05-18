# Operating Model

How I❤️NDB runs day to day, using this SSOT repo.

## The brain

This repo is the brain:
- `memory/` — what is true and what is approved.
- `skills/` — how each output type is produced.
- `prompts/` — how to run Hermes anywhere.
- `campaigns/` — ready packs.
- `docs/` — tone, risk, policy, roles.
- `evidence/` — proof per gate.

## Daily cycle

1. Bootstrap Hermes (`prompts/hermes_bootstrap_prompt.md`).
2. Run the daily operator prompt (`prompts/daily_operator_prompt.md`).
3. Hermes drafts content using `skills/` + `memory/` + `docs/`.
4. Founder reviews → approves → publishes.
5. Approved text logged in `memory/approved_messages.md`.

## Weekly cycle

1. Run the weekly review prompt (`prompts/weekly_review_prompt.md`).
2. Honest review + next 3 priorities.
3. Founder decides direction.

## Gate cycle

1. A gate (e.g. `INDB-HERMES-SSOT-0`) defines a unit of work.
2. Claude Code builds it and writes `evidence/<GATE>/proof.md`.
3. Pass/fail checklist recorded. Then the next gate.

## Roles in one line

Founder gates · Hermes drafts · Claude Code builds · ChatGPT reviews.
(Full detail: `docs/claude_vs_hermes_roles.md`.)

## Principle

Keep it simple and markdown-first. The model is memory → message → action →
proof. Do not over-build.
