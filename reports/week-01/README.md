# Week 01 report

## Project

Running Coach App, team 4.

Our problem-space sentence: a recreational runner training for a 5K to half-marathon race, often without a sports watch, needs a training plan that changes when their real runs differ from the plan and tells them why it changed, so they can trust it enough to keep following it.

## What we did

We searched 18 candidates and researched four alternatives: Runna (`ALT-01`, direct competitor), Garmin Coach (`ALT-02`, direct competitor bound to Garmin hardware), Hal Higdon plans (`ALT-03`, adjacent substitute), and GoldenCheetah (`ALT-04`, open source).
We compared them on seven properties fixed in advance, found three gaps, rejected five candidates, and proposed two value propositions.
We held the kickoff meeting with the Customer on TODO(date).

## Findings

Runna is the product we could lose to: it works from a phone, adapts to skipped runs, and is the only product in our set that shows why a change happened, but only for pace changes from speed sessions.
Garmin Coach adapts the most, but only on a recent Garmin watch, and its documentation does not say whether the runner sees a reason.
Where training load is measured (Garmin, GoldenCheetah), it is not documented as changing the plan.
We therefore propose `VP-01`, a plan that explains every change it makes, and `VP-02`, adaptation from phone-only and walk/run runs.

<!-- TODO(team): add one or two sentences on what the kickoff changed, e.g. "The Customer narrowed the target runner to ... and moved VP-02 out of scope". -->

## Coverage

| Deliverable | Artifact |
| --- | --- |
| Candidate list | [candidate-list.md](candidate-list.md) |
| Alternatives search | [docs/research/alternatives.md](../../docs/research/alternatives.md) |
| Compare the alternatives | [docs/research/comparison.md](../../docs/research/comparison.md) |
| Gap analysis | [docs/research/gap-analysis.md](../../docs/research/gap-analysis.md) |
| Value proposition | [docs/research/value-proposition.md](../../docs/research/value-proposition.md) |
| Research board | TODO(team): view-only board link |
| Meeting script | [meeting-script.md](meeting-script.md) |
| Customer kickoff | [meeting-report.md](meeting-report.md), [meeting-transcript.md](meeting-transcript.md) |
| AI usage | [ai-usage.md](ai-usage.md) |

The repository is licensed under the [MIT License](../../LICENSE).

## Repository evidence

<!-- TODO(team): after the PRs are merged and the link check is green on main, replace these with real links (full URLs to github.com). -->

- Branch protection on `main` (pull request required, one approval, no self-approval): TODO(team) save the screenshot as `images/branch-protection.png`, then replace this text with `![Branch protection settings for main](images/branch-protection.png)`.
- Merged pull request approved by another member: TODO(PR link)
- Latest green link check on `main`: TODO(Actions run link)
- Excluded links: none.
  <!-- If you add an entry to .lycheeignore, say here which link, why it cannot be checked mechanically, and that you opened it in a browser on <date>. -->

## Contribution

<!-- TODO(team): replace usernames and links. Every member needs at least one commit through a PR and one approval of someone else's PR. -->

| Member | Work |
| --- | --- |
| @JustACommonMan-OSDD | TODO: PR #, what it added, approved PR # of @Sirjaey |
| @Sirjaey | TODO |
| @Obetech1 | TODO |
| @Ezekiel-Gadzama | TODO |

## Deviations

None.

<!-- TODO(team): if the meeting was asynchronous, or you wrote notes instead of a transcript, declare it here with the reason. -->

## Privacy

No private-only material was committed to this repository.
