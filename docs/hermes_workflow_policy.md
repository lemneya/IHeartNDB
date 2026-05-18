# Hermes Workflow Policy

Governs **how Hermes output enters the IHeartNDB SSOT repo**. The goal: keep
the SSOT clean. Hermes is productive but must not pollute authoritative folders
with raw, unreviewed files.

Established by gate: `INDB-HERMES-WORKFLOW-1`.

---

## What Hermes may produce

Hermes may generate **drafts, analyses, briefs, and campaign ideas**:
- post drafts, WhatsApp messages, comment replies
- comment/sentiment analyses
- daily and weekly briefs
- campaign concepts and pack proposals

Producing these is allowed and encouraged. **Where they land is controlled.**

---

## The pipeline (one direction only)

```
Hermes writes  →  hermes_inbox/      (raw, unreviewed, allowed to be messy)
Claude reviews →  proposes promotion (organize, classify, recommend)
Founder        →  approves authoritative / public-facing content
Promoted to    →  approved/  or  memory/  or  campaigns/
Rejected/old   →  archive/
```

Nothing skips a stage. Output does not jump straight from Hermes into `memory/`
or into public use.

---

## Folder contract

| Folder | Owner | Holds | Rule |
|---|---|---|---|
| `hermes_inbox/` | Hermes (write) | Raw Hermes output: drafts, analyses, briefs | **Only place Hermes writes.** May be messy. Not authoritative. |
| `hermes_inbox/analysis/` | Hermes | Sentiment/comment analyses | Raw until reviewed. |
| `hermes_inbox/briefs/` | Hermes | Daily/weekly briefs | Raw until reviewed. |
| `approved/` | Founder-approved | Content cleared for use | Entered **only after founder approval**. |
| `approved/posts/` | Founder-approved | Approved post content | — |
| `approved/briefs/` | Founder-approved | Approved briefs | — |
| `approved/analysis/` | Founder-approved | Approved analyses | — |
| `memory/` | SSOT (protected) | Authoritative facts, identity, approvals | **Never raw Hermes output.** Curated, founder-backed only. |
| `campaigns/` | SSOT | Structured campaign packs | Reviewed, formatted packs only. |
| `archive/` | Cold storage | Outdated or rejected material | Kept, not deleted. Provenance preserved. |

---

## Roles in this workflow

- **Hermes** — writes to `hermes_inbox/` only. Never writes to `memory/`,
  `campaigns/`, `approved/`, or repo root.
- **Claude** — reviews items in `hermes_inbox/`, organizes them, and **proposes**
  promotion (to `approved/`, `memory/`, `campaigns/`) or archival. Claude does
  not approve public content and does not auto-publish.
- **Founder (Mohiyidine Cheikh)** — approves public-facing or authoritative
  content. Only founder-approved material reaches `approved/` or `memory/`.

---

## Hard constraints

1. **No automatic publishing.** Nothing goes public without founder approval.
2. **No automatic deletion.** Unwanted material is moved to `archive/`, never
   deleted, unless the founder explicitly orders deletion in a later gate.
3. **`memory/` is protected.** It is the authoritative SSOT, not scratch space.
   Raw Hermes output must never be committed directly into `memory/`.
4. **One-way flow.** `hermes_inbox/` → review → approved/memory/campaigns, or
   → archive. Never the reverse without a new gate.
5. **Provenance preserved.** Promotions and archivals keep a trace (commit
   message and/or `evidence/`), so the origin of authoritative content is
   auditable.

---

## Why this exists

During `INDB-HERMES-SSOT-0` a background Hermes process wrote
`memory/facebook_comments_analysis.md` and `briefs/daily_brief_today.md`
directly into the working tree. Useful content, wrong location. This policy
gives Hermes a sanctioned inbox so the SSOT stays trustworthy.
