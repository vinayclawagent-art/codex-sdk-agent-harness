# Evidence-Backed Preset: Repo Hygiene Maintenance Bot

Source package: [[../../Generated-Packages/Codex SDK Agent Harness/README|Codex SDK Agent Harness]]
Loop: [[../../Improvement-Loops/Codex SDK Agent Harness Loop|Codex SDK Agent Harness Loop]]

## Preset status

- Status: template ready; needs a real repo trial before being called validated
- Date prepared: 2026-06-06
- Intended runner: Codex Python SDK task harness
- Evidence standard: record command output, diff summary, evaluator, and decision before shipping any automated change

## Harness preset

### Use case
Embed Codex into a repeatable repo hygiene pass that finds stale README instructions, missing run commands, and untracked TODO drift before a human release or demo.

### Risk / bottleneck
Maintenance agents can over-edit prose, hide risky assumptions, or create noisy diffs if the harness does not force source evidence and a human accept/reject gate.

### Output mode
Structured markdown report plus optional patch proposal. The harness should default to report-only until the repo owner approves a patch.

## Suggested harness fields

| Field | Value |
| --- | --- |
| `task_name` | `repo-hygiene-maintenance` |
| `mode` | `report-first` |
| `allowed_paths` | `README.md`, `docs/**`, `.github/ISSUE_TEMPLATE/**`, `package.json`, `pyproject.toml` |
| `blocked_paths` | `.env*`, secrets, production configs, credentials, deployment keys |
| `max_diff_files` | `5` |
| `human_gate` | required before commit or push |

## Evidence capture template

```markdown
# Repo Hygiene Trial Evidence

Repo:
Date:
Harness command:
Input scope:

## Raw observations
- 

## Proposed diff summary
- Files touched:
- Risk level:
- Tests or checks run:

## Human evaluation
- Accepted:
- Rejected:
- Required edits:

## Follow-up
- Promote preset? yes/no
- Convert into Hermes skill? yes/no
```

## Done condition for the next run

This preset counts as complete only when one real repo trial attaches command output, a diff summary, and a human decision. Until then it remains a prepared preset, not proof of automation performance.
