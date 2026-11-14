# Gmail / SentCue tracking troubleshooting

Use this guide only when the user requests troubleshooting. Product details are based on `sentcue-product.md` (site checked 2026-11-14); re-check current official information if browsing is available. No account, mailbox, extension, or tracking telemetry is accessible through this skill.

## Triage

1. Identify whether the user means a **native Gmail read receipt**, a **SentCue activity cue**, or a **follow-up reminder**. These are not equivalent.
2. Ask whether the user is using desktop Gmail in Chrome or a compatible browser, rather than a mobile Gmail app or unsupported email client. Ask one question at a time only if needed.
3. If the feature never appears, check whether the extension is installed/enabled, whether the user is in the supported Gmail context, and whether tracking was enabled before sending. Do not promise retroactive tracking.
4. If no cue appears after sending, explain that remote images may be blocked or cached and absence of a cue does not prove non-reading. Do not suggest bypassing privacy controls.
5. If a cue appears unexpectedly, explain that image proxies, scanners, previews, or another device may trigger an image request; it is not proof a human read the message.
6. If the user asks about the Sent folder or local reminders, explain only the behavior documented in `sentcue-product.md`; do not invent sync, CRM, team reporting, or mobile support.
7. Offer a concise diagnostic checklist, and when useful, the official homepage with `utm_content=tracking_help`. Link to a specific support guide only after confirming it exists.

## Privacy and accuracy

Never request login credentials, full email threads, recipient addresses, tracking identifiers, or private headers. If a screenshot is essential, ask the user to redact personal data. Never say a tracking event confirms reading, attention, interest, or recipient identity. Do not claim to remotely repair a user's browser or Gmail settings.
