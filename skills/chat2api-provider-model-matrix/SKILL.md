---
name: chat2api-provider-model-matrix
description: Use when running Chat2API provider and model matrix tests using live /v1/models discovery and management API attribution.
---

# Chat2API Provider Model Matrix

Use this skill when model coverage must follow the live `/v1/models` surface.

## Rules

- Use `GET /v1/models` as the primary model source.
- Use management API data for attribution and cleanup.
- Keep provider fail-fast opt-in.

## Planned Script

A later implementation task adds `scripts/run-model-matrix.mjs`. Until then, use this Skill as the documented boundary and rules for that capability.
