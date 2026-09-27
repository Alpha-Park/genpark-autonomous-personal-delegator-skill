---
name: genpark-autonomous-personal-delegator-skill
description: GenPark AI Agent Skill - Autonomous micro-action delegation with user guardrails, confidence thresholding, dry-run previews, and token budget gating.
version: 1.0.0
category: Service
author: GenPark AI Ecosystem (@alphaparkinc)
---

# GenPark Autonomous Personal Delegator Skill Specification

## Core Directives
1. Maintain strict user privacy boundaries; context telemetry must not capture sensitive passwords, credentials, or private keys.
2. Provide deterministic confidence intervals for all predictive actions.
3. Require explicit confirmation if an action impact is non-reversible.

## MCP Tools
- **evaluate_delegation_safety**: Scores proposed autonomous actions against user risk boundaries, reversible impact levels, and required permissions.
- **stage_micro_action**: Stages non-destructive micro-actions in a dry-run state awaiting automatic or single-click confirmation.
- **execute_sandboxed_dispatch**: Executes verified micro-actions across connected agent tools within strict token and latency budgets.
