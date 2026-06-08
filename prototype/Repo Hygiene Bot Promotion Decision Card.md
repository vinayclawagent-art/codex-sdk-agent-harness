---
type: promotion-decision-card
status: ready-for-trial
package: "[[Codex SDK Agent Harness]]"
source_note: "[[Codex Python SDK for Programmatic Coding Agents]]"
created: 2026-06-08
tags: [promotion-card, codex, coding-agents, x-artifact-factory]
---
# Repo Hygiene Bot Promotion Decision Card

Use this after the next **real** repo hygiene trial uses [[Repo Hygiene Trial Kickoff Card]] and [[Evidence-Backed Preset - Repo Hygiene Maintenance Bot]]. The card turns the trial result into a promote / pilot-only / iterate / hold decision without claiming validation before code, logs, or human review exist.

## Candidate metadata

- Target repo:
- Branch / workspace:
- Max diff budget:
- Blocked paths:
- Report artifact link:
- Reviewer:
- Date reviewed:

## Evidence checklist

- [ ] Trial ran on a real repository or a clearly named sandbox clone of one.
- [ ] Kickoff card records scope, blocked paths, and max-diff guardrails before edits.
- [ ] Agent output includes a report-first summary before any patch/commit decision.
- [ ] Evidence preset captures commands run, files inspected, proposed diffs, and reviewer decision.
- [ ] Any code changes were either applied on an allowed branch or explicitly left as recommendations.
- [ ] Human review outcome is recorded before promotion.

## Decision — choose exactly one

| Choice | Use when | Selected |
|---|---|---|
| Promote to reusable harness | Report-first flow, guardrails, and evidence fields worked on a real repo and can be reused. | [ ] |
| Pilot-only | The bot is useful for selected repos but still needs constraints or examples. | [ ] |
| Iterate preset/card | Scope, blocked paths, evidence capture, or diff budget were incomplete/confusing. | [ ] |
| Hold | The trial produced no safe/useful repo maintenance result. | [ ] |

## Promotion guardrails

- Do **not** promote `codex-sdk-task-harness` until a real repo trial fills both kickoff and evidence artifacts.
- Do **not** report repo-safety validation unless the blocked-path and max-diff fields were set before the run.
- Do **not** count speculative patches as success; require command output, reviewed diff, or an explicit no-change report.
- Keep this card blank and reusable until the next real trial supplies evidence.

## Follow-up updates after decision

- [ ] Update [[Codex SDK Agent Harness Loop]] with the selected outcome.
- [ ] Update [[Artifacts/Generated-Packages/Codex SDK Agent Harness/README]] changelog.
- [ ] If promoted, refine or install the skill draft with the proven guardrails.
- [ ] If iterating, adjust the preset/card before another repo trial.

## Outcome log

- Decision:
- Rationale:
- Evidence links:
- Next owner:
- Next trial date:
