# New Chat Handoff — Tinker

## Objective
Define objective for Tinker

## Targets
- (none)

## Current Status
- Initialized context handoff workflow.

## Context Window Watch
- Status: **UNKNOWN** (usage not provided)
- Thresholds: warning at 70.0% | critical at 85.0%
- Immediate instruction:
  - Continue current work.
  - Re-check context after each major block (or every 3-5 tool calls).
- Trigger plan:
  - At WARNING (70% = 190400 tokens): checkpoint + summarize + prep handoff.
  - At CRITICAL (85% = 231200 tokens): stop and switch chat immediately.
  - Pass --tokens-used to calculate next trigger distance.

## Model Awareness
- Active model: **GPT-5.3-Codex**
- Approx context window: **272000 tokens**
- Cost multiplier hint: (not set)
- Notes: Approximate Copilot input context.

## Key Sources
- (none)

## Next Actions
- Define immediate next action.

## Blockers
- (none)

## Notes
- 2026-02-15T08:06:05+00:00 | Bootstrapped project-level context handoff tooling

## Workspace Artifacts
- CONTEXT_HANDOFF.md
- .context_handoff_state.json
- CONTEXT_HANDOFF_WORKFLOW.md

_Generated: 2026-02-15T08:06:05+00:00_
