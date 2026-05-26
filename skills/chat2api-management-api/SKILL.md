---
name: chat2api-management-api
description: Use when operating Chat2API Manager's management API for testing, including health checks, config snapshots, temporary API keys, model mappings, sessions, logs, and cleanup verification.
---

# Chat2API Management API

Use this skill before live proxy testing that needs `/v0/management/*`.

## Rules

- Never print full management secrets, API keys, or account credentials.
- Create disposable API keys for tests and delete only keys created by the current run.
- Snapshot config before mutation and restore it in cleanup.
- Do not clear sessions unless the user explicitly asks for cleanup.

## Planned Script

A later implementation task adds `scripts/management-api.mjs`. Until then, use this Skill as the documented boundary and rules for that capability.
