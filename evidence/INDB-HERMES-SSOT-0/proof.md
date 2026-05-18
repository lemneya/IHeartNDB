# Proof Pack — Gate INDB-HERMES-SSOT-0

**Gate:** INDB-HERMES-SSOT-0
**Objective:** Create the foundational single source of truth (SSOT) repo for
the Hermes-I❤️NDB Civic Operator agent.
**Built by:** Claude Code (repo builder role)
**Date:** 2026-05-18
**Status:** ✅ PASS — foundation established, no app code created.

---

## 1. File tree created

```
README.md                          ← I❤️NDB / Hermes SSOT overview, current gate
AGENTS.md                          ← Hermes-I❤️NDB Civic Operator definition

memory/
  I_LOVE_NDB_CAMPAIGN.md           ← founder, movement, economic-capital memory
  city_identity.md                 ← Nouadhibou identity, voice, brand
  campaign_principles.md           ← 10 fixed principles
  approved_messages.md             ← founder-approval log (CP-001 pending)
  founder_notes.md                 ← founder intent + working agreement

skills/
  facebook_post_writer.md
  whatsapp_campaign_message.md
  comment_reply.md
  issue_brief.md
  daily_briefing.md
  avatar_presenter_script.md
  weekly_campaign_review.md

campaigns/
  001_nouadhibou_remembers.md      ← full Campaign Pack 001
  002_economic_capital.md          ← full Campaign Pack 002
  003_clean_ndb.md                 ← full Campaign Pack 003

prompts/
  daily_operator_prompt.md
  weekly_review_prompt.md
  avatar_presenter_prompt.md
  hermes_bootstrap_prompt.md       ← copy-paste Hermes loader
  campaign_pack_prompt.md

docs/
  tone_guide.md
  risk_policy.md
  whatsapp_policy.md
  operating_model.md
  claude_vs_hermes_roles.md
  public_claims_policy.md

evidence/
  .gitkeep
  INDB-HERMES-SSOT-0/
    proof.md                       ← this file

(legacy, kept as working drafts, not authoritative)
  content/posts/sample-nouadhibou-soul.md
  system/system-prompt.md  system/tone-guide.md
  templates/avatar-script.md  templates/comment-reply.md
  templates/facebook-post.md  templates/whatsapp-message.md
```

All required files and folders from the gate spec exist.

---

## 2. Role separation confirmed

Defined and authoritative in `docs/claude_vs_hermes_roles.md`:

- **Founder (Mohiyidine Cheikh)** = vision, approval, **final gate**.
- **Hermes** = campaign operator: memory, daily content, civic messaging.
  Drafts only; never publishes; never commits code.
- **Claude Code** = repo builder: structure, commits, proof packs, technical
  organization. Does not write as Hermes; does not approve.
- **ChatGPT** = gatekeeper, strategist, reviewer, prompt architect.

Confirmed: roles are explicitly separated and the founder gate is mandatory
before any public output. ✅

---

## 3. First campaign pack created

`campaigns/001_nouadhibou_remembers.md` ("نواذيبو تتذكر / Nouadhibou
Remembers") contains all required components:

- [x] Arabic Facebook post
- [x] Hassaniya-style WhatsApp short message
- [x] French summary
- [x] English summary
- [x] Banner slogan
- [x] 45-second avatar presenter script (timecoded)
- [x] Comment reply template (+ hostile-comment note)
- [x] One action people can take today
- [x] One metric to track
- [x] Approval block (PENDING — founder)

Two additional packs (002 economic capital, 003 clean NDB) also created in the
same format. All marked **DRAFT — needs founder approval**.

---

## 4. Risks documented

`docs/risk_policy.md` documents and prohibits:

- [x] Political escalation
- [x] Accusing specific people without evidence
- [x] Fake statistics
- [x] Religious/political manipulation
- [x] Spam
- [x] WhatsApp must be respectful and consent-aware (`docs/whatsapp_policy.md`)
- [x] Public content must be approved before publishing

Supported by `docs/public_claims_policy.md` (verified-only claims) and
`docs/tone_guide.md` (no insults, unify not divide).

---

## 5. Pass/Fail checklist

| # | Check | Result |
|---|---|---|
| 1 | README explains I❤️NDB, Hermes, repo purpose, role separation, current gate | ✅ PASS |
| 2 | AGENTS.md defines mission, languages, tone, all 7 hard rules | ✅ PASS |
| 3 | memory/I_LOVE_NDB_CAMPAIGN.md has founder, movement, economic-capital reasons, why it exists, love→action | ✅ PASS |
| 4 | docs/claude_vs_hermes_roles.md cleanly separates Founder / Hermes / Claude Code / ChatGPT | ✅ PASS |
| 5 | docs/risk_policy.md covers all required risk items | ✅ PASS |
| 6 | campaigns/001 has all 9 required components + approval block | ✅ PASS |
| 7 | prompts/hermes_bootstrap_prompt.md is a working copy-paste loader | ✅ PASS |
| 8 | evidence/INDB-HERMES-SSOT-0/proof.md present with tree, roles, pack, risks, checklist | ✅ PASS |
| 9 | Markdown-first, no app code, no unnecessary frameworks | ✅ PASS |
| 10 | All 7 skills + 5 prompts + 6 docs + 5 memory + 3 campaigns present | ✅ PASS |

**Gate result: ✅ PASS — INDB-HERMES-SSOT-0 complete.**

Next: commit as the SSOT foundation. No app code created in this gate, by
design and by founder instruction.
