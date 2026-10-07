# Week 02 report

## Project

Running Coach App, team 4.

Our problem-space sentence: a recreational runner training for a 5K to half-marathon race, often without a sports
watch, needs a training plan that changes when their real runs differ from the plan and tells them why it
changed, so they can trust it enough to keep following it.

The 2 October kickoff overrode the second half of that sentence.
This week we wrote down what the kickoff actually asked for: [the product vision](../../docs/product-vision.md)
goals on [VP-01](../../docs/research/value-proposition.md#vp-01), the in-run voice coach, with
[VP-02](../../docs/research/value-proposition.md#vp-02) as two preset sessions spoken by that coach.

## What we found out we were wrong about

We built Week 1 toward a training plan that adapts and explains itself.
The `Customer` did not mention a plan once in twenty-nine minutes.
This week we stopped defending it: an adaptive plan, and the explanation of a plan change, are now outside the
product in [`BND-01`](../../docs/product-vision.md#bnd-01) and [`BND-02`](../../docs/product-vision.md#bnd-02),
and [`GAP-01`](../../docs/research/gap-analysis.md#gap-01) and
[`GAP-03`](../../docs/research/gap-analysis.md#gap-03) sit in the research unaddressed rather than closed.

What we were right about, and now have evidence for, is that the runner is a beginner to intermediate with only
a phone. Those survived as [`DEC-001`](../../docs/decisions.md#dec-001) and
[`DEC-002`](../../docs/decisions.md#dec-002).

Still open is [`ASM-07`](../../docs/assumptions.md#asm-07) — whether an adaptive plan is wanted at all — which
action point A2 puts to the `Customer` in this week's meeting.

## What we did

Converted the Week 1 research to the identifier format the updated requirements ask for, and created the two logs
Week 1 did not have: [`docs/decisions.md`](../../docs/decisions.md) with `DEC-001` to `DEC-006`, one per kickoff
decision, and [`docs/assumptions.md`](../../docs/assumptions.md) with `ASM-01` to `ASM-08`.

Wrote [`docs/product-vision.md`](../../docs/product-vision.md): a goal that traces to `VP-01`, five stakeholders,
eight `CON-nn` constraints, six `BND-nn` boundary items, and a system context diagram.

Prototyped the part we are least sure about — whether fixed spoken cues are enough for a first release — and put
the mock, the boundary, and the candidate into [the meeting script](meeting-script.md).

Added the Markdown check and its configuration.

## Coverage

| Deliverable            | Artifact                                                                                                            |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------- |
| Kickoff action points  | `## Previous action points` in `reports/week-02/meeting-report.md`                                                  |
| Kickoff open questions | `## Previous open questions` in `reports/week-02/meeting-report.md`                                                 |
| Product vision         | `docs/product-vision.md`                                                                                            |
| System context diagram | `docs/architecture/context.svg` and its source `docs/architecture/context.mmd`, embedded in `docs/product-vision.md` |
| Assumptions            | `docs/assumptions.md`                                                                                               |
| Decisions              | `docs/decisions.md`                                                                                                 |
| Story issues           | [the `US-nn` issues, filtered by the `user-story` label](https://github.com/Running-Coach-App/running-coach-app/issues?q=label%3Auser-story) |
| Issue forms            | `.github/ISSUE_TEMPLATE/user-story.yml`, `.github/ISSUE_TEMPLATE/task.yml`, and `.github/ISSUE_TEMPLATE/config.yml`  |
| Labels                 | [the repository's labels page](https://github.com/Running-Coach-App/running-coach-app/labels), with `user-story`, `task`, and the `moscow:*` labels |
| Pull request template  | `.github/pull_request_template.md`                                                                                  |
| Prototypes             | `reports/week-02/prototypes.md`                                                                                     |
| Meeting script         | `reports/week-02/meeting-script.md`                                                                                 |
| Customer validation    | `reports/week-02/meeting-report.md`, and `reports/week-02/meeting-transcript.md` when there is one                    |
| AI usage               | `reports/week-02/ai-usage.md`                                                                                       |

## Minimum Usable Product Candidate

Core task: a runner puts the phone in a pocket, starts a session, and hears what to do and how it is going until
they stop.

- [`US-01`: Start and stop a run without touching the phone](https://github.com/Running-Coach-App/running-coach-app/issues?q=is%3Aissue+US-01)
- [`US-02`: Hear the run's stats spoken while running](https://github.com/Running-Coach-App/running-coach-app/issues?q=is%3Aissue+US-02)
- [`US-04`: Choose one of two preset sessions](https://github.com/Running-Coach-App/running-coach-app/issues?q=is%3Aissue+US-04)

`US-03` sits outside the candidate although it is `Must Have`: the cue that names the interval depends on
`US-04`'s session to fire against, and we would rather show a runner that the phone can talk than that it can
count.

Customer's verdict: _**to fill in after the meeting**_ — its `DEC-nnn` goes here, per
[The Candidate](../../.claude/skills/itpd/requirements/minimum-usable-product-requirements.md#the-candidate).

## Repository evidence

_Merged pull request closing its task issue, latest green link check run, and latest green Markdown check run:_
_to be added once this week's pull requests are merged._

## Contribution

| Member                | Work                                                                                              |
| --------------------- | ------------------------------------------------------------------------------------------------- |
| @Ezekiel-Gadzama      |                                                                                                   |
| @sirjaey              |                                                                                                   |
| @Obetech1             |                                                                                                   |
| @JustACommonMan-OSDD  |                                                                                                   |

## Deviations

1. **The story and task issues are not open yet.**
   The session that produced this work has no GitHub credentials, so `.github/ISSUE_TEMPLATE/` and the
   `user-story`, `task`, and `moscow:*` labels could not be created through the API, and issues could not be
   opened from the forms.
   The bodies are prepared outside the repository — deliberately outside it, because
   [`Where Stories Live`](../../.claude/skills/itpd/requirements/user-stories-requirements.md#where-stories-live)
   rule 5 forbids keeping a second list of stories in the repository — and will be pasted into the forms when a
   member with access opens them.
   Every story body, its `AC-nn` criteria, and its priority reason are written.

2. **The Markdown check disables three rules.**
   `MD013` and `MD029` are turned off because
   [`Continuous Integration`](../../.claude/skills/itpd/requirements/repository-requirements.md#continuous-integration)
   requires exactly that of them: one sentence per line and long table rows, and a meeting script that numbers
   its questions across its agenda groups.
   `MD036` is also off, because the research requirements require `**Strengths**` and
   `**Observations by property**` as bare bold lines and `MD036` reads a bare bold line as a mistyped heading.
   The two directly conflict, and the requirement wins.
   Nothing else is excluded; `.claude/skills/itpd/**` is excluded as the course materials' directory.

3. **The prototype's HTML source is not committed.**
   [`Where Prototypes Live`](../../.claude/skills/itpd/requirements/prototypes-requirements.md#where-prototypes-live)
   rule 4 keeps disposable prototype code off `main` in Week 2, so the evidence is the screenshot and
   [`prototypes.md`](prototypes.md), not the file it was screenshotted from.

4. **`reports/week-02/meeting-report.md` does not exist yet.**
   The validation meeting has not been held, so there is no report, no transcript, no verdict `DEC-nnn`, and no
   record of what the prototype changed. This section is incomplete until it is.

## Privacy

No private-only material was committed to this repository.
