---
type: improvement-loop
status: active
package: "[[Codex SDK Agent Harness]]"
source_note: "[[Codex Python SDK for Programmatic Coding Agents]]"
github_repo: "https://github.com/vinayclawagent-art/codex-sdk-agent-harness"
cadence: nightly
last_improved: 2026-06-06
next_focus: "Run the Repo Hygiene Maintenance Bot preset on one real repo and attach command output, diff summary, evaluator, and decision."
tags: [improvement-loop, x-artifact-factory]
---
# Codex SDK Agent Harness Loop

Package: [[Codex SDK Agent Harness]]
GitHub: https://github.com/vinayclawagent-art/codex-sdk-agent-harness

## Current improvement
- 2026-06-06: Created first-pass prototype and repo mirror.
- 2026-06-06: Added [[../Prototypes/codex-sdk-agent-harness/Evidence-Backed Preset - Repo Hygiene Maintenance Bot|Evidence-Backed Preset - Repo Hygiene Maintenance Bot]] with report-first defaults, blocked paths, max-diff guardrails, and an evidence template for the first real trial.

## Next focus
Run the Repo Hygiene Maintenance Bot preset against one real VinClawLabs repo; attach command output, diff summary, evaluator, decision, and follow-up.

## Backlog
- Add one source-specific preset. ✅ Prepared via the Repo Hygiene Maintenance Bot preset.
- Add evidence fields: input, output, evaluator, decision, follow-up. ✅ Template prepared; do not mark validated until a real run fills it.
- Decide whether the skill draft is reusable enough to promote.
