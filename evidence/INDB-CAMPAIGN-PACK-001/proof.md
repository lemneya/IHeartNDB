# Proof Pack — Gate INDB-CAMPAIGN-PACK-001 (Restore + Verify)

**Gate:** INDB-CAMPAIGN-PACK-001 — restore and verify Hermes campaign draft
**Reviewed file:** `hermes_inbox/briefs/campaign_pack_001b_nouadhibou_remembers.md`
**Reviewer:** Claude Code (verification role — NOT founder, NOT approval)
**Date:** 2026-05-18
**Final verification result: ⚠️ PASS WITH EDITS**

---

## 0. Restoration disclosure (mandatory context)

- The campaign pack **had been removed** before this verification: in a prior
  turn the user instructed "REMOVE IT" and the file was deleted. It was never
  git-tracked, so there was no recoverable git history.
- It was **restored verbatim** from content captured in a system-reminder
  (the 159-line user/linter-modified version). **No rewriting, no improving,
  no content changes** were made during restoration.
- Restoration was performed **only to allow this verification** to run, on
  explicit user instruction (chose "Restore, then verify").
- The file **remains UNAPPROVED** and **inside `hermes_inbox/`**. It was **not**
  moved to `approved/`, **not** copied to `memory/` or `campaigns/`, and
  **not** published. Founder approval is **PENDING**.
- Restored file integrity: 159 lines, 6153 bytes, located exactly at
  `hermes_inbox/briefs/campaign_pack_001b_nouadhibou_remembers.md`.

> Claude does not approve on behalf of the founder. This proof is a review only.

---

## 1. File existence — PASS

`hermes_inbox/briefs/campaign_pack_001b_nouadhibou_remembers.md` exists at the
correct path (159 lines / 6153 bytes). ✅

---

## 2. Required sections (11/11) — PASS

| # | Section | Found at line | Result |
|---|---|---|---|
| 1 | Arabic Facebook post | 11 | ✅ |
| 2 | Hassaniya-style WhatsApp short message | 34 | ✅ |
| 3 | French summary | 50 | ✅ |
| 4 | English summary | 62 | ✅ |
| 5 | Banner slogan | 73 | ✅ |
| 6 | 45-second avatar presenter script | 82 | ✅ |
| 7 | Comment reply template | 106 | ✅ |
| 8 | One action people can take today | 123 | ✅ |
| 9 | One metric to track | 130 | ✅ |
| 10 | Risk check section | 137 | ✅ |
| 11 | Founder approval block | 151 | ✅ |

All 11 required sections present. ✅

---

## 3. Risk review

| Risk | Finding | Result |
|---|---|---|
| Political attacks | None. No party, official, or institution targeted. | ✅ PASS |
| Accusations without evidence | None. No person/body blamed. | ✅ PASS |
| Fake numbers | **Zero statistics used** anywhere in the pack. | ✅ PASS |
| Overclaiming | Mostly safe ("كانت تُذكر كـ" / "remembered as" / "restée dans la mémoire comme"). **Two assertive lines**: WhatsApp "العاصمة الاقتصادية ... هي حقيقة بنيناها بيدينا" and banner "ليست ذكرى، بل واجب" lean from *remembered* toward *asserted*. Civic rhetoric, not a legal claim — but flag for softening. | ⚠️ EDIT |
| Unsafe WhatsApp / spam | WhatsApp asks to share with **one** person — consent-aware, not mass-blast. Not spam. | ✅ PASS |
| Tone mismatch | Warm, patriotic, emotional, practical, unifying — matches `docs/tone_guide.md`. No insults. | ✅ PASS |
| Unclear action | §8 canonical action is single and clear. **But** WhatsApp (§2) bundles two micro-steps (forward to one person **and** post a photo). Inconsistent with the "one clear action" rule. | ⚠️ EDIT |

No hard-rule violation. Two items need founder edits, none blocking.

---

## 4. Language quality review

| Dimension | Assessment |
|---|---|
| Arabic emotional strength | **Strong.** "نواذيبو ليست مجرد اسم على الخريطة" + "البحر الذي أطعم بيوتنا، والأيادي التي بنت اقتصاد موريتانيا بصمتٍ وكرامة" — evocative, dignified, on-voice. ✅ |
| Hassaniya naturalness | **Acceptable.** WhatsApp register ("اللي طعمت أهلها", "خلّينا نفكّروها ونخدمو عليها", "هاذ الرسالة", "وزيد صورة") reads as authentic Hassaniya-flavored colloquial. Could be slightly more idiomatic but natural enough. ✅ |
| French clarity | **Clear & grammatical.** "Nouadhibou est restée dans la mémoire comme la capitale économique … refusons l'oubli." ✅ |
| English clarity | **Clear & clean.** "remembered as Mauritania's economic capital … let's not let it fade." ✅ |
| Safe framing of "العاصمة الاقتصادية" | **Mostly safe.** Arabic FB ("كانت تُذكر كـ"), French ("restée dans la mémoire comme"), English ("remembered as") all frame it as a *remembered civic/economic role* — compliant with `docs/public_claims_policy.md`. **Exception:** WhatsApp "هي حقيقة بنيناها بيدينا" and banner "ليست ذكرى، بل واجب" assert it more strongly. No source is cited for an official/legal status (correctly — none is claimed), but these two lines should be softened to stay within remembered/earned framing. ⚠️ EDIT |

---

## 5. Recommended founder edits (non-blocking)

1. **Hashtag consistency / platform safety (highest priority).** This pack uses
   `#نواذيبو_تتذكّر` (with a shadda ّ on ـذ). Pack 001 uses `#نواذيبو_تتذكر`
   (no shadda). A combining diacritic inside a hashtag is unreliable on
   Facebook/WhatsApp (may split or drop the tag) and fragments the campaign
   tag. **Recommend: standardize to `#نواذيبو_تتذكر` (no shadda)** everywhere
   in this pack to match Pack 001.
2. **Soften two assertive economic-capital lines** to match the safe
   remembered/earned framing used elsewhere and `docs/public_claims_policy.md`:
   - WhatsApp: "...العاصمة الاقتصادية ما هي كلمة، هي حقيقة..." → e.g.
     "...حقيقة نتذكّرها ونعتز بها..."
   - Banner: optional — "ليست ذكرى، بل واجب" is acceptable civic rhetoric;
     soften only if the founder prefers strict remembered-framing.
3. **Tighten the WhatsApp action to one step.** Currently: forward to one
   person **and** post a photo with the hashtag. Reduce to a single action to
   honor the "one clear action" rule and match §8.
4. **Content-overlap observation (founder decision, not a risk).** Per its own
   header (`Source: Campaign Pack 001 + Facebook comments analysis`), 001B's
   Arabic post, French/English summaries, avatar script, and comment reply are
   **near-verbatim to Pack 001**. The founder should confirm whether 001B is
   intended as a *refined variant of 001* or should be made *distinct* before
   approval/promotion.
5. **Internal label note.** The approval block lists `Gate:
   INDB-CAMPAIGN-PACK-001`; harmless, but the founder may want the pack's
   internal gate label kept consistent with whatever gate finally approves it.

---

## 6. Pass / Fail checklist

| Check | Result |
|---|---|
| File restored verbatim (no rewrite/improve) | ✅ PASS |
| File exists at correct inbox path | ✅ PASS |
| All 11 required sections present | ✅ PASS |
| No political attacks | ✅ PASS |
| No accusations without evidence | ✅ PASS |
| No fake numbers | ✅ PASS |
| No spam / WhatsApp consent-aware | ✅ PASS |
| Tone matches `docs/tone_guide.md` | ✅ PASS |
| Arabic / Hassaniya / French / English quality | ✅ PASS |
| "العاصمة الاقتصادية" safely framed | ⚠️ MOSTLY (2 lines to soften) |
| Single clear action | ⚠️ §8 ok; WhatsApp bundles 2 steps |
| Hashtag consistent & platform-safe | ⚠️ EDIT (shadda vs Pack 001) |
| Not approved / not published / stays in `hermes_inbox/` | ✅ PASS |
| Founder approval status | ⬜ PENDING — Mohiyidine Cheikh (NOT given) |

---

## 7. Final verification result

# ⚠️ PASS WITH EDITS

The pack is safe, on-tone, complete, and violates no hard rule. It is **not**
ready for unconditional approval: apply the recommended edits (especially the
hashtag diacritic fix and the two economic-capital softenings) before the
founder approves and before any promotion out of `hermes_inbox/`.

**Founder approval remains PENDING. Claude has not approved and has not
published. The file stays in `hermes_inbox/` unapproved.**
