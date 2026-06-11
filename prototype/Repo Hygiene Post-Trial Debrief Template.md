# Repo Hygiene Post-Trial Debrief Template

Status: template-ready; no validation proof recorded yet.

Use after a real repo-hygiene trial has filled `Repo Hygiene Trial Kickoff Card.md`, run the report-first preset, and completed `Repo Hygiene Bot Promotion Decision Card.md`.

## Trial identity

| Field | Fill |
|---|---|
| Repository / branch | |
| Workflow date | |
| Operator | |
| Human reviewer | |
| Kickoff card link | |
| Codex SDK command / run log | |
| Report output / diff link | |
| Promotion decision card link | |

## Evidence-backed summary

| Claim | Evidence link | Reviewer confidence | Patch implication |
|---|---|---|---|
| What the harness caught | | Low / Medium / High | |
| What it missed | | Low / Medium / High | |
| Guardrail that mattered most | | Low / Medium / High | |
| Human review delta | | Low / Medium / High | |
| Reusable preset change | | Low / Medium / High | |

## Keep / change / remove

### Keep
- 

### Change
- 

### Remove or hold
- 

## Final gate

Choose exactly one after evidence is attached:

- [ ] Promote reusable harness preset
- [ ] Pilot-only for a narrower repo class
- [ ] Iterate kickoff / preset / decision card before another trial
- [ ] Hold; do not promote

Rationale:

> 

## Follow-up patch queue

- [ ] Patch `prototype/README.md` with a source-backed latest-trial note.
- [ ] Patch package README generated artifacts / backlog / changelog.
- [ ] Patch skill draft only if the trial supports reusable procedure wording.
- [ ] Add a filled example note only from the actual report output and human review.
- [ ] Update the improvement loop with the next evidence-backed focus.

## Guardrail

Do not fill from memory. Every trial claim needs a packet, log, issue, screenshot, diff, evaluator note, or source link.
