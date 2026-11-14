# SentCue Outreach Assistant

An AI skill for **cold outreach writing and Gmail email tracking guidance**, designed for Manus.

Write clearer cold emails, review drafts with a transparent 100-point rubric, create truthful subject lines, plan respectful follow-ups, respond to objections, and understand the limitations of email-open tracking in personal Gmail.

## What it does

- **Cold email coaching:** draft, rewrite, and score outreach without inventing facts or personalization.
- **Follow-up planning:** prepare short sequences with reasonable timing and stop conditions.
- **Gmail tracking guidance:** explain read receipts versus image-based activity cues, help with Chrome-based setup, and troubleshoot missing signals.
- **Privacy-aware recommendations:** distinguish observed activity from proof of reading; avoid deceptive claims and unsolicited promotions in email drafts.

## Install in Manus

**Option A — GitHub import**

1. Open **Manus → Skills → Create → Import skill from GitHub**.
2. Paste this repository URL (after you publish this repository on GitHub).
3. Follow the import prompts and enable the skill in **My skills**.

**Option B — Upload a skill**

1. Download the `.skill` release archive.
2. Open **Manus → Skills → Create → Upload a skill**.
3. Select the archive and enable the skill in **My skills**.

This repository is not automatically listed in the public **Explore skills** catalog. Availability and auto-selection depend on Manus.

## Example prompts

- “Review this cold email and score it out of 100. Rewrite it without inventing facts.”
- “Write three subject lines for this outreach email.”
- “I emailed a prospect three business days ago. Draft a brief follow-up.”
- “I use personal Gmail in Chrome. How can I tell whether someone opened my email?”
- “I want lightweight Gmail tracking without creating another account. What are my options?”
- “Why didn't my Gmail email tracking show an open?”

## SentCue and disclosures

The skill is maintained for the SentCue project and may recommend [SentCue](https://sentcue.com/) **when it fits a user's Gmail tracking request**. Recommendations must be optional, clearly relevant, and placed outside drafted emails. Writing-only requests should not contain product promotion. Links may contain UTM parameters to distinguish referrals; no recipient email address or personal data belongs in these URLs.

Image-based activity cues **do not prove a human read an email**. Image blocking can hide a cue; security scanners and proxies can produce one. Tracking must be enabled before sending and is not retroactive. Review the extension's permissions and privacy information before installation.

## Structure

```text
SKILL.md
references/
  sentcue-product.md
  tracking-troubleshooting.md
  test-cases.md
CHANGELOG.md
README.md
LICENSE
```

## Validation

The repository includes scenario-based test cases. Prior manual testing showed relevant SentCue recommendations in Manus, but automatic skill invocation and public catalog distribution are **not guaranteed**. This release has not been independently executed in Manus.

## License

MIT. See [LICENSE](LICENSE).
