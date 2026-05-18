# I ❤️ NDB — Hermes Civic Operator SSOT

This repository is the **single source of truth (SSOT)** for the I❤️NDB civic movement
and the **Hermes-I❤️NDB Civic Operator** agent.

> This repo is **not an app**. It is the campaign **brain, memory, prompt library,
> skills library, and proof folder** for the I❤️NDB movement. Markdown first.
> No app code yet.

---

## What is I❤️NDB?

I❤️NDB is a **civic pride and action movement** for **Nouadhibou (نواذيبو)**, Mauritania.

It exists to protect and amplify the **memory, dignity, economy, environment,
culture, and future** of Nouadhibou — the city long remembered as Mauritania's
**economic capital** because of its port, fish, trade, industry,
mining/logistics position, and strategic location.

People are starting to forget that role. I❤️NDB turns **love of the city into
visible action**.

Founder: **Mohiyidine Cheikh**.

---

## Why Hermes?

**Hermes** is the always-on **civic operator**. The founder cannot personally write
every post, reply, brief, and briefing every day. Hermes carries the campaign's
memory and voice so the movement can speak **consistently, respectfully, and
daily** — while the founder keeps the **final approval gate**.

Hermes never publishes on its own. Hermes drafts; the founder approves.

---

## Why this repo exists

- To hold the **memory** of the campaign so nothing depends on one person's recall.
- To hold a **skills library** so every output type is produced the same way.
- To hold a **prompt library** so Hermes can be bootstrapped anywhere, anytime.
- To hold a **proof folder** so every gate is auditable.

If this repo is lost, the campaign loses its brain. Treat it as the SSOT.

---

## How Claude, Hermes, and the Founder work separately

| Actor | Role |
|---|---|
| **Founder (Mohiyidine Cheikh)** | Vision, approval, final gate. Nothing goes public without him. |
| **Hermes-I❤️NDB** | Campaign operator. Memory, daily content, civic messaging. |
| **Claude Code** | Repo builder. Structure, commits, proof packs, technical organization. |
| **ChatGPT** | Gatekeeper, strategist, reviewer, prompt architect. |

Full separation: [`docs/claude_vs_hermes_roles.md`](docs/claude_vs_hermes_roles.md)

These roles never merge. Claude Code does not write campaign messages as if it were
Hermes. Hermes does not commit code. The founder does not get bypassed.

---

## Repository map

```
README.md                  → this file
AGENTS.md                  → Hermes operator definition
memory/                    → campaign brain (facts, identity, approvals)
skills/                    → how to produce each output type
campaigns/                 → ready campaign packs
prompts/                   → copy-paste prompts to run Hermes
docs/                      → tone, risk, policy, operating model
evidence/                  → proof packs per gate
content/  system/  templates/  → legacy working drafts (kept, not authoritative)
```

The authoritative material is `memory/`, `skills/`, `campaigns/`, `prompts/`,
`docs/`. The older `content/`, `system/`, `templates/` folders are kept as
working drafts and historical reference.

---

## Hermes output workflow

To keep the SSOT clean, Hermes never writes directly into authoritative
folders. Output flows one way:

```
Hermes outputs   → hermes_inbox/
Claude review    → approved/  or  memory/  (proposed, then approved)
Founder approval → public use
```

- `hermes_inbox/` — raw Hermes drafts, analyses, briefs (may be messy).
- `approved/` — founder-approved content ready for use.
- `archive/` — outdated or rejected material (kept, not deleted).
- `memory/` — protected SSOT; never receives raw Hermes output.

Full policy: [`docs/hermes_workflow_policy.md`](docs/hermes_workflow_policy.md).

---

## Current gate

**`INDB-HERMES-SSOT-0`** — Create the foundational single source of truth repo.

Proof: [`evidence/INDB-HERMES-SSOT-0/proof.md`](evidence/INDB-HERMES-SSOT-0/proof.md)

Status: this gate establishes the brain. No app code is created in this gate.
