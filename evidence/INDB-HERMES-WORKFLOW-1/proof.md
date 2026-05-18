# Proof Pack — Gate INDB-HERMES-WORKFLOW-1

**Gate:** INDB-HERMES-WORKFLOW-1
**Objective:** Control how Hermes writes outputs into the IHeartNDB repo so the
SSOT is not polluted by random background files.
**Built by:** Claude Code (repo builder role)
**Date:** 2026-05-18
**Status:** ✅ PASS — controlled Hermes workflow established. No content deleted.

---

## Trigger

Background Hermes process had created an **untracked** file:
`memory/facebook_comments_analysis.md` (6021 bytes) — useful content, wrong
(protected SSOT) location.

Decision applied: do **not** delete, do **not** commit it in place — instead
move it into a sanctioned inbox and define a one-way workflow.

---

## 1. File moved

| From | To | Result |
|---|---|---|
| `memory/facebook_comments_analysis.md` | `hermes_inbox/analysis/facebook_comments_analysis.md` | ✅ Moved, 6021 bytes preserved, content intact |

`memory/` now contains only the 5 authoritative SSOT files (no raw Hermes
output):
`approved_messages.md`, `campaign_principles.md`, `city_identity.md`,
`founder_notes.md`, `I_LOVE_NDB_CAMPAIGN.md`.

---

## 2. Folders created

```
hermes_inbox/
  .gitkeep
  analysis/
    .gitkeep
    facebook_comments_analysis.md   ← moved file lives here
  briefs/
    .gitkeep

approved/
  .gitkeep
  posts/.gitkeep
  briefs/.gitkeep
  analysis/.gitkeep

archive/
  .gitkeep
```

All 8 required `.gitkeep` anchors created. ✅

---

## 3. Policy created

`docs/hermes_workflow_policy.md` — defines:
- Hermes may produce drafts, analyses, briefs, campaign ideas.
- Hermes output goes **first** into `hermes_inbox/`.
- Claude reviews and proposes promotion.
- Founder approves public-facing / authoritative content.
- Only approved material moves into `approved/` or `memory/`.
- `memory/` is authoritative — never receives raw Hermes output.
- `campaigns/` = structured campaign packs.
- `approved/` = founder-approved, ready for use.
- `archive/` = outdated/rejected, kept not deleted.
- No automatic publishing. No automatic deletion.

✅ All required points present.

---

## 4. README updated

Added **"Hermes output workflow"** section with the one-way flow:
`Hermes outputs → hermes_inbox/` · `Claude review → approved/ or memory/` ·
`Founder approval → public use`, plus folder roles and a link to the policy. ✅

---

## 5. AGENTS updated

Added **"Repo Write Discipline"** section:
- Hermes writes to `hermes_inbox/` only.
- Claude organizes and proposes promotion.
- Founder approves final public content.
- `memory/` is protected SSOT, not scratch space.
- No automatic publishing / deletion.

✅ Section present and linked to the policy.

---

## 6. No content deleted

- The Hermes file was **moved**, not deleted (byte size unchanged: 6021).
- `briefs/daily_brief_today.md` from the prior gate left untouched.
- Legacy `content/`, `system/`, `templates/` left untouched.
- `archive/` exists for future rejected material — nothing archived yet.

✅ Zero deletions.

---

## 7. git status before commit (clean except expected files)

```
 M AGENTS.md                         ← expected (Repo Write Discipline section)
 M README.md                         ← expected (workflow note)
?? approved/                         ← expected (new folder)
?? archive/                          ← expected (new folder)
?? docs/hermes_workflow_policy.md    ← expected (new policy)
?? hermes_inbox/                     ← expected (new folder + moved file)
```

No unexpected files. The previously-untracked `memory/facebook_comments_analysis.md`
no longer appears under `memory/` (relocated, as intended). ✅

---

## Pass/Fail checklist

| # | Check | Result |
|---|---|---|
| 1 | `hermes_inbox/` + `analysis/` + `briefs/` created with `.gitkeep` | ✅ PASS |
| 2 | `approved/` + `posts/` + `briefs/` + `analysis/` created with `.gitkeep` | ✅ PASS |
| 3 | `archive/` created with `.gitkeep` | ✅ PASS |
| 4 | Untracked Hermes file moved to `hermes_inbox/analysis/` (not deleted) | ✅ PASS |
| 5 | `docs/hermes_workflow_policy.md` created with all required content | ✅ PASS |
| 6 | AGENTS.md has "Repo Write Discipline" section | ✅ PASS |
| 7 | README.md has the workflow note | ✅ PASS |
| 8 | `memory/` holds no raw Hermes output | ✅ PASS |
| 9 | No content deleted anywhere | ✅ PASS |
| 10 | git status clean except expected files before commit | ✅ PASS |

**Gate result: ✅ PASS — INDB-HERMES-WORKFLOW-1 complete.**
