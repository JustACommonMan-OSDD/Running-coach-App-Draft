# Value Proposition

Each value proposition closes at least one gap from [the gap analysis](gap-analysis.md), names what it costs, and says how a competitor would respond.

The 2 October kickoff changed which proposition leads. The customer asked for a voice in the ear during the run. [GAP-01](gap-analysis.md#gap-01-the-runner-is-not-told-why-the-plan-changed) was not confirmed, so a plan that explains its own changes is not a proposition in this file. Phone-only and beginner-to-intermediate did survive, and that is the user in [GAP-02](gap-analysis.md#gap-02-no-adaptation-from-how-a-phone-recorded-run-actually-went).

## VP-01: A voice coach during the run

**User:** a beginner to intermediate runner, often without a sports watch, who will not keep looking at the phone.
**Problem:** the products he can already use show pace, distance, and heart rate on a screen. He has to take the phone out to know them, and nothing talks him through the run.
**What we do:** during the run the phone speaks encouragement, a simple intensity cue (hard, then easier, then jog), and the stats it already has: time, pace, distance, and heart rate when a connected device provides it. He can set how often the stats are spoken. After the run it speaks a short summary. The first release is English, on Android, and processes on the phone where we can.
**Measured by:** on a phone with no watch, the runner hears time, pace, and distance at least once every three minutes without opening the screen, and hears the hard/easy cue in a preset interval session.
**Closes:** the phone-only beginner in [GAP-02](gap-analysis.md#gap-02-no-adaptation-from-how-a-phone-recorded-run-actually-went). The kickoff replaced that gap's closing test. He wants the phone to speak the run back while he is running, not a perceived-effort rating that rewrites the next session.
**What it costs:** without a watch we cannot promise heart rate, so the coach speaks time, pace, and distance, and adds heart rate only when a wearable is connected. Keeping the processing on the phone limits how capable the spoken coach can be. We give up an adaptive training plan in the first release so this can ship.
**How a competitor would respond:** Runna (ALT-01) and Garmin Coach (ALT-02) already own plan adaptation and could add spoken stats in a release. The customer uses Google Health and dislikes it because it makes him stare at the stats and does not talk. Spoken stats are not a deep moat. They are the part he said his current app does not do.

## VP-02: Two preset sessions, after the voice coach

**User:** the same runner, once VP-01 works.
**Problem:** he does not want to design each interval himself, and he has not seen a goal-setting screen he trusts. He asked for a small number of programmes the app proposes, after the talking coach is in place.
**What we do:** offer two preset sessions the coach speaks, for example a steady run and a hard/easy interval, and he picks one. This release does not build a weekly plan that rewrites itself.
**Measured by:** the runner can start either preset and hear that session's cues without looking at the phone.
**Closes:** the walk/run beginner in [GAP-02](gap-analysis.md#gap-02-no-adaptation-from-how-a-phone-recorded-run-actually-went), as a fixed spoken session rather than a post-run rewrite. [GAP-01](gap-analysis.md#gap-01-the-runner-is-not-told-why-the-plan-changed) and [GAP-03](gap-analysis.md#gap-03-training-load-is-measured-but-not-connected-to-the-plan) stay open until the next meeting.
**What it costs:** two presets cannot serve a runner who wants a race plan. We give up granular goal setting, meal advice, and automatic plan edits.
**How a competitor would respond:** Runna (ALT-01) and Hal Higdon (ALT-03) already ship full plans. They do not need to answer two spoken presets. Copying their plans is not this proposition.

## Assumptions

Rows D1 to D6 were said at the 2 October kickoff. The record is the [meeting report](../../reports/week-01/meeting-report.md).

| Assumption | Supports | How to check, and when |
| --- | --- | --- |
| The first audience is beginner to intermediate. Marathon and professional runners are out of the first release. | VP-01 | Recorded as D1. |
| The product must work from the phone. A watch is optional and only adds signals such as heart rate. | GAP-02, VP-01 | Recorded as D2. |
| Runners will not upload medical documents or type extra health data in. Inputs come from the phone, and from a wearable only if one is already connected. | VP-01 | Recorded as D3. No perceived-effort step in the first release. |
| Processing stays on the phone where we can. | VP-01 | Recorded as D4. |
| Sharing stats with a friend is out of scope for these ten weeks. | scope | Recorded as D5. |
| The first release is Android and English. | VP-01 | Recorded as D6. |
| The base product is the in-run voice coach. A preset session comes after that. | VP-01, VP-02 | Said at the 2 October kickoff. Confirm on Tuesday 6 October that he does not also want an adaptive plan (meeting report A2). |
| Fixed spoken cues are acceptable for the first release. A conversational model was his suggestion and was not settled. | VP-01 | Ask on Tuesday 6 October (meeting report A4). |
