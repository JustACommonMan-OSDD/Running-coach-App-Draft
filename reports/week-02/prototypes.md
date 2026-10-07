# Week 02 prototypes

## Spoken cue walkthrough

- **What it is:** a static three-screen mock of what the runner hears — before the run, during it, and after it — with the coach's line shown as the loudest block on each screen.
- **View:** [the mock](images/voice-cue-prototype.png).
- **Tested:** [`US-02`](https://github.com/Running-Coach-App/running-coach-app/issues), [`US-03`](https://github.com/Running-Coach-App/running-coach-app/issues), and [`US-05`](https://github.com/Running-Coach-App/running-coach-app/issues), exercising `AC-01` of each; and [`ASM-08`](../../docs/assumptions.md#asm-08), because whether fixed cues are enough to ship is the risky part, not whether speech can be produced.
- **Question:** will he accept fixed spoken cues for the first release, or does he need the model to talk back?
- **What the customer said:**
  > **To fill in after the meeting.** The script puts this at agenda part 2, question 2, and it is the question `ASM-08` rests on.
- **What changed:**
  > **To fill in after the meeting.** Whatever he says becomes a `DEC-nnn` in [`docs/decisions.md`](../../docs/decisions.md), is listed under `## Decisions` in `reports/week-02/meeting-report.md`, and lands in `ASM-08` as `Confirmed` or `Refuted` and in the affected story issue.

## Why this and not something else

`Validation` rule 2 says to build the thing we are least sure about.
We are not unsure that a phone can speak a number — that is settled engineering.
We are unsure that he will accept the first release without a model listening, and that is what the mock shows:
the fixed cue in the middle screen, with the note under it saying plainly that nothing is listening.

The mock is deliberately not beautiful and does not need to work.
It exists so he can react to the part we got wrong rather than to the part we got right.

## Disposal

The mock's HTML source is not committed.
`Where Prototypes Live` rule 4 keeps disposable prototype code off `main` in Week 2, and the evidence for this
week is this record and its screenshot.
