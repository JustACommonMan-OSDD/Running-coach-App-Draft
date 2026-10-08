# Week 2 TODO

Deadline: soft **Thu 8 Oct 23:59**, hard **Sat 10 Oct 23:59**.
Checked against `assignment-2.md` (submodule at `a949e8d`, current).
State as of now, branch `sirjaey`, everything committed.

Only box you can tick on your own right now is the first one. The rest need a push, the GitHub web UI, or the meeting.

## On your own, right now

- [x] Scaffolds created: `reports/week-02/meeting-report.md` (all 8 sections, 6 action-point rows, 5 open-question rows) and `reports/week-02/meeting-transcript.md` (format + example lines). They are untracked (`??` in `git status`).
- [ ] Nothing else — every step below this line is blocked on a push, on GitHub, or on the meeting.

## Push and pull requests (you — needs your credentials)

- [ ] `git push origin sirjaey` — the `week 2` commit `b9d12e1` is local only.
- [ ] Open the **blank issue first** (`config.yml` disables blank issues once merged, so this order matters), then the forms PR from it (Part 1, Issue Tracking rule 2). Name that issue's task and close it like any other.
- [ ] Checklist wants separate PRs in order, not one big merge: (1) Week 1 research restructure (items 7–8), (2) issue forms (item 1), (3) `markdown.yml` + config (item 9, after PR 1 merges so CI is green on first run), (4) vision + week-02 files.
- [ ] Each PR must close exactly one task issue via `Closes #nn`; reviewer ticks its `AC-nn` boxes before approving.
- [ ] Confirm the checks run: a Markdown check and the lychee link check must both go green on `main` before submission (item 9).

## GitHub web UI (you — no API access from here)

- [ ] Create 6 labels: `user-story`, `task`, `moscow:must`, `moscow:should`, `moscow:could`, `moscow:won't` (item 1).
- [ ] Open 10 story issues from `user-story.yml`, bodies in `week-02-story-issues.md` (outside the repo on purpose — rule 5 forbids a second list in the repo). Apply one `moscow:*` label each (item 11).
- [ ] Open the 4 task issues from `task.yml` (same file). `Story` stays empty for non-story work.
- [ ] After issues exist, replace the placeholder links: candidate `US-01/02/04` links in `reports/week-02/README.md`, the `US-nn` links in `reports/week-02/meeting-script.md` agenda part 4, and the `US-02/03/05` links in `reports/week-02/prototypes.md` — all currently point at `/issues`.

## The meeting (the team — cannot be written in advance)

- [ ] Hold the validation meeting. Checklist item 16's script is ready; agenda part 4 lists the candidate `US-nn`.
- [ ] Fill in `reports/week-02/meeting-report.md`: 6 `## Previous action points` rows (A1–A6), 5 `## Previous open questions` rows, Summary, 2+ Decisions (one = the candidate verdict), 2+ action points due Week 3, Open questions, Disagreements. Every `TODO` must be gone. Delete the scaffold note at the top.
- [ ] Fill in or delete `reports/week-02/meeting-transcript.md`. If recording was refused: delete it, say so in the report.
- [ ] Record each decision as a `DEC-nnn` entry in `docs/decisions.md` and list it in the report.
- [ ] Change **at least one artifact** because of what he said about the prototype, citing its `DEC-nnn` in the artifact, the report, and `prototypes.md` (item 19) — this is the bolded checklist item.
- [ ] Settle `ASM-07`/`ASM-08` to `Confirmed` or `Refuted` with `Outcome:` if the meeting decides them; record the candidate verdict's `DEC-nnn` in the README's MUP section.
- [ ] Fill in the Contribution table in `reports/week-02/README.md` — currently 4 empty rows.

## Submission (you — last)

- [ ] Merge everything to `main`. Take permalink + snapshot from that commit; check the rendered permalink.
- [ ] Build the 2-page Moodle PDF (project + team, member table, permalink, recording link or one line why none, transcript appendix if refused, privacy line).
- [ ] Verify Deviations item 1 (no GitHub access) and item 4 (report written after meeting) are resolved or rewritten; keep items 2–3 as written.
- [ ] Final local gate before pushing: `markdownlint-cli2 "**/*.md"` 0 errors, all internal anchors resolve.