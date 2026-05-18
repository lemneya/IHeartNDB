# Legacy Review — Pre-SSOT Drafts

Purpose: assess the folders/files that existed **before** the
`INDB-HERMES-SSOT-0` SSOT foundation, and recommend what to do with each.

> **No file is moved, archived, or deleted by this review.** This is an
> assessment only. Actions happen in a later, separately approved gate.

Reviewed at: gate INDB-HERMES-SSOT-0 follow-up · Date: 2026-05-18
Scope: `content/`, `system/`, `templates/` (the legacy folders from commit
`d9fc154` "initial I❤️NDB campaign repo").

---

## 1. Existing legacy folders/files found

| Path | What it is |
|---|---|
| `content/posts/sample-nouadhibou-soul.md` | A drafted Arabic Facebook post ("نواذيبو روح") with visual + call to action. |
| `system/system-prompt.md` | Old Hermes system prompt ("Hermes-I❤️NDB Civic Operator", role, rules, formula). |
| `system/tone-guide.md` | Old tone guide (voice, spelling, reply style, formula, forbidden list). |
| `templates/avatar-script.md` | Avatar script skeleton (scenes, timecodes, CTA). |
| `templates/comment-reply.md` | Comment-reply skeleton (acknowledge → amplify → reaffirm). |
| `templates/facebook-post.md` | Facebook post skeleton (emotion → message → visual → CTA). |
| `templates/whatsapp-message.md` | WhatsApp message skeleton (greeting → hook → info → action). |

---

## 2. Assessment (useful / duplicate / outdated / unclear)

| Path | Assessment | Reasoning |
|---|---|---|
| `content/posts/sample-nouadhibou-soul.md` | **Useful (sample)** | Real, on-tone draft content. Not yet a SSOT campaign pack and not in `memory/approved_messages.md`. Value as a reference sample, not as authoritative. |
| `system/system-prompt.md` | **Duplicate** | Superseded by `AGENTS.md` + `prompts/hermes_bootstrap_prompt.md`, which are broader and current. Content is consistent (no contradiction), just older/narrower. |
| `system/tone-guide.md` | **Duplicate** | `docs/tone_guide.md` was built from this and extends it (Hassaniya, languages, brand). Same voice, no conflict; the new file is the source of truth. |
| `templates/avatar-script.md` | **Duplicate** | Superseded by `skills/avatar_presenter_script.md` (same structure + process + checklist). |
| `templates/comment-reply.md` | **Duplicate** | Superseded by `skills/comment_reply.md`. |
| `templates/facebook-post.md` | **Duplicate** | Superseded by `skills/facebook_post_writer.md`. |
| `templates/whatsapp-message.md` | **Duplicate** | Superseded by `skills/whatsapp_campaign_message.md`. |

No legacy file **contradicts** the SSOT. The risk is **drift/confusion from
two copies**, not conflicting guidance.

---

## 3. Recommendation (keep / migrate / archive / delete later)

| Path | Recommendation | Detail (for a later approved gate) |
|---|---|---|
| `content/posts/sample-nouadhibou-soul.md` | **Migrate** | Promote into `campaigns/` as a sample pack, or log to `memory/approved_messages.md` only after founder approval. Keep the content; relocate it. |
| `system/system-prompt.md` | **Archive** | Historical origin of the operator definition. Move under an `archive/` (or `evidence/`) folder rather than delete, to preserve provenance. |
| `system/tone-guide.md` | **Archive** | Same — provenance of `docs/tone_guide.md`. |
| `templates/avatar-script.md` | **Archive then delete later** | Fully superseded by the matching skill. Archive once, then remove in a later cleanup gate. |
| `templates/comment-reply.md` | **Archive then delete later** | Superseded by `skills/comment_reply.md`. |
| `templates/facebook-post.md` | **Archive then delete later** | Superseded by `skills/facebook_post_writer.md`. |
| `templates/whatsapp-message.md` | **Archive then delete later** | Superseded by `skills/whatsapp_campaign_message.md`. |

Suggested sequencing for the future cleanup gate:
1. Migrate the sample post into the SSOT (founder approval first).
2. Archive `system/` and `templates/` (preserve provenance, stop drift).
3. Delete archived duplicates only after the founder confirms.

---

## 4. Status of this review

- Nothing moved.
- Nothing archived.
- Nothing deleted.
- Legacy `content/`, `system/`, `templates/` remain exactly as they are.
- Action requires a separate, founder-approved cleanup gate.

> Continuity note — `daily_brief_today.md`: this was an external
> Hermes-generated draft that entered the repo during the SSOT gate at
> `briefs/daily_brief_today.md` (outside `hermes_inbox/`). Under gate
> **INDB-HERMES-CLEANUP-1** (2026-05-18) it has been **relocated** to
> `hermes_inbox/briefs/daily_brief_today.md` for review, in line with
> `docs/hermes_workflow_policy.md`. The content was **moved, not deleted**, and
> the now-empty `briefs/` folder was removed (its role is served by
> `hermes_inbox/briefs/`). It awaits Claude review and founder approval before
> any promotion to `approved/`, `memory/`, or `campaigns/`.
