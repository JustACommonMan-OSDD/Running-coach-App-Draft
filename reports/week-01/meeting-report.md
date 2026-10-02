# Kickoff meeting report

## Metadata

| | |
| --- | --- |
| Date | Friday 2 October 2026 |
| Duration | 29 minutes |
| Attended | `Customer`; `@Ezekiel-Gadzama` (interviewer); `@Obetech1`; `@Sirjaey`; `@JustACommonMan-OSDD` (timekeeper) |
| We presented | Nothing from our Week 1 research was presented. The `Customer` opened by describing the product himself, and the meeting became a question-and-answer session. Neither the rule-based engine nor the `VP-01` explanation screen was put to him. |
| Recording | Permitted; Zoom produced an automatic transcript. |
| Transcript may be published | TODO: confirm with the `Customer` before committing `meeting-transcript.md`. Until he confirms, keep `meeting-notes.md` instead. The recording file stays out of the repository. |

## Summary

The `Customer` described a product that is not the one our Week 1 research assumed.

Our research built toward a **training plan** that adapts after a missed or difficult week and explains why it changed (`GAP-01`, `VP-01`). The `Customer` described a **real-time running companion**: a voice in your ear that varies the intensity during the run ("30 seconds as hard as you can, then medium, then just jog"), reads your pace, distance and heart rate back to you at intervals so you never look at the phone, and sends a summary at the end. He said he uses Google Health and dislikes it for exactly one reason — "it all requires me staring at stats on the phone, it doesn't talk to me."

He did not mention race training, weekly plans, or plan changes at any point in 29 minutes. The nearest he came was in answer to `@Obetech1`'s question about goal setting, where he said he prefers a small number of preset programmes over granular user controls, and placed that explicitly *after* the talking-coach base: "if we can just do that and report it back to user, it would be nice... that would be the base, and then on top of that, if we can offer a programme."

Two parts of our research did survive contact, both from the `VP-02` side: the target runner is a beginner, and the product must work from the phone alone.

This divergence is the main outcome of the meeting and is carried into Open questions below.

## Decisions

| # | Decision | Comes from | Evidence |
| --- | --- | --- | --- |
| D1 | Target runner is **beginner to intermediate**. Marathon runners may have training requirements the `Customer` does not know, and are not the audience for the first release. | `VP-02` — confirms the user in the proposition | 24:06 |
| D2 | **Phone-only is the baseline.** Take whatever the phone gives (motion sensors, microphone, GPS); a wearable such as a watch "would be a good thing to explore" but is not required. | `GAP-02`, `VP-02` — confirms the no-watch premise | 11:03–12:05 |
| D3 | **No upload of health or medical documents.** The `Customer` judges that users are unwilling — "too lazy, or they think it's a security problem". Inputs come from the device only. | New constraint; narrows `VP-02` inputs | 11:34–11:50 |
| D4 | **Processing stays on the phone where possible**, rather than sending the run to the cloud. | New constraint; reinforces `VP-02` | 15:02–15:17 |
| D5 | **No social or friend-sharing features** in the ten weeks. The `Customer` judged shared stats "a project on its own" and ruled it out of scope, while leaving it open for later. | Scope boundary | 09:12–09:25 |
| D6 | **Android, English, first release.** The `Customer` has no iOS device and cannot test one. Publishing to the Android store, or as open source on GitHub, both acceptable. | Platform constraint | 22:09, 23:30–23:50 |

## Action points

| # | Action | Owner | Due |
| --- | --- | --- | --- |
| A1 | Rewrite the problem-space sentence and re-score the gap analysis against a real-time audio coach, then decide whether `VP-01` survives as our lead proposition or is replaced. | `@Ezekiel-Gadzama` | Mon 5 Oct 2026 |
| A2 | Put the divergence to the `Customer` directly at the next meeting: show him `VP-01` and ask whether an adaptive training plan is wanted at all, or whether the in-run coach is the whole product. | `@Ezekiel-Gadzama` | Tue 6 Oct 2026 |
| A3 | Confirm the next meeting slot offline and send the invitation. The `Customer` asked for 08:00 WAT if the team can manage it; the team offered 08:30. | `@JustACommonMan-OSDD` | Mon 5 Oct 2026 |
| A4 | Ask the `Customer` whether a rule-based engine is acceptable rather than machine learning. The assumption table lists this as "present it at the Week 1 kickoff"; it was not asked. | `@Sirjaey` | Tue 6 Oct 2026 |
| A5 | Research on-device text-to-speech and small-model options for Android, starting from the `Customer`'s own suggestion of Gemma, and report feasibility within the ten weeks. | `@Obetech1` | Thu 8 Oct 2026 |
| A6 | Ask the three unasked starred questions from `meeting-script.md` (Q3, Q7, Q10) at the next meeting. | `@Ezekiel-Gadzama` | Tue 6 Oct 2026 |

## Open questions

| Question | What it would change | Follow-up |
| --- | --- | --- |
| Does the `Customer` want an adaptive **training plan** at all, or only the in-run coach? | Decides whether `GAP-01` and `VP-01` stay in the project. If he does not want a plan, there is nothing to explain, and our lead proposition has no customer. | A2, next meeting |
| Rule-based engine or machine learning? | `VP-01` depends on a rule-based engine being acceptable, because the explanation names the rule that fired. | A4 |
| Which ships first if only one can: the explanation of a plan change, or phone-only adaptation? | Week 5 scope. Script question 10, not asked. | A6 |
| Are professional runners in scope later? | The `Customer` asked *us* whether we know what professional runners need, and no one answered. Affects whether the plan engine must generalise. | Next meeting |
| What does a wearable add, and can we reach one in ten weeks? | Whether heart rate is an input at all. The `Customer` called it worth exploring but was not confident. | A5 |
| Is a published transcript permitted? | Whether this repository carries `meeting-transcript.md` or `meeting-notes.md`. | Before committing either |

## Disagreements

One, and it was resolved in the meeting.

`@Ezekiel-Gadzama` proposed that runners be able to see a running partner's live stats — heart rate, average speed — while running together. The `Customer` accepted the idea but refused it for this project on effort grounds: sharing, unsharing and securing data between accounts is "quite complex... a project on its own", and he doubted it could be reached in ten weeks. He left it open as a possible paid tier if the team continues after the course. Recorded as `D5`.

No other disagreement. The `Customer` twice stepped out of the customer role to say that the project is "just a vehicle for you to practise processes" and that where it is published matters less than that it is published.
