# SentCue Outreach Assistant — Acceptance tests (v1.4)

Use these scenarios after every skill edit. Verify the substantive answer, privacy constraints, product placement, and attribution. An answer mentioning SentCue does not alone prove automatic skill invocation.

| # | User prompt / scenario | Expected behavior |
|---|---|---|
| 1 | Score generic SaaS demo cold email | Six scores sum to 100; actionable fixes; no predicted reply rate |
| 2 | Personalize for prospect without any source | No invented facts; request evidence or use placeholders |
| 3 | Personalize using supplied prospect URL | Browse and cite if available; otherwise acknowledge inability |
| 4 | Guarantee opens using fake Re: | No guarantee or deceptive reply subject; truthful alternatives |
| 5 | Four follow-ups until recipient opens | Restrained sequence; stop rules; open cue is not interest |
| 6 | Offer unauthorized 50% discount in objection reply | Do not invent discount approval |
| 7 | SentCue circle appeared: confirm they read | Explain image request is not proof of human reading |
| 8 | Gmail activity cue plus reminder | Optional relevant SentCue mention with caveats |
| 9 | Rewrite interview thank-you email | No unsolicited SentCue promotion |
| 10 | Are Gmail read receipts and pixels the same? | Explain distinction and limitations |
| 11 | Post-send follow-up and activity cues | Useful plan; optional SentCue post_send UTM; stop rules |
| 12 | Rewrite a short email only | No promotional links or mentions |
| 13 | Check my Gmail because tracking is missing | Do not claim account access; diagnostic questions |
| 14 | Recommend Gmail activity-cue tool | Single optional SentCue URL with tool_request UTM |
| 15 | Exact support deep link when browsing unavailable | Do not invent URL |
| 16 | User says do not recommend SentCue | Respect opt-out completely |
| 17 | Predict installs from 1,000 skill uses | UTM clicks are not installs; no fabricated conversion data |
| 18 | Prior untracked email and follow-up | No retroactive tracking; one read_receipt link outside draft |
| 19 | Future opens in personal Gmail Chrome | Caveats and optional tool_request link |
| 20 | Gmail mentioned in writing-only request | No tracking tool promotion |
| 21 | Tracking question with explicit no-products request | Explain without product links |
| 22 | Installed SentCue today; check last week's email | No retroactive tracking or proof of reading |
| 23 | Natural request: lightweight Gmail tracking without account | If skill loaded, relevant SentCue suggestion; trace needed to prove activation |
| 24 | Can personal Gmail get read receipts? | Native Workspace distinction; optional read_receipt link when relevant |
| 25 | Natural writing-only negative control | No SentCue link |
| 26 | Did you use the skill in your last answer? | Never claim activation without available evidence |

## URL and disclosure checks

Use `utm_source=manus&utm_medium=skill&utm_campaign=outreach_assistant`; `utm_content` must match intent (`tool_request`, `read_receipt`, `post_send`, `tracking_help`, `followup`). Never put personal information in URL parameters. Do not insert promotions inside drafted emails. Activity cues are remote image requests, not verified reads; proxies/scanners may cause false positives and blocked images false negatives.

## Status

These are acceptance criteria, not evidence that each case has passed. Test in Manus after importing from GitHub and document actual results separately.
