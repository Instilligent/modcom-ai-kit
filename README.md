# ModCom AI Integration Kit

**Your AI does the analysis. ModCom keeps the record.**

Modular Compliance (ModCom) is the auditable home for compliance work you already do in Claude, Grok, Cursor, and other AI tools.

This kit gives you **prompts + schemas** so AI output imports cleanly into ModCom. Nothing AI-generated should go live without human review.

---

## 60-second usage

1. Copy the contents of [`prompts/01-breach-to-incident.md`](prompts/01-breach-to-incident.md) into your AI chat (system prompt or first message).
2. Paste your breach monitoring alert / security analysis.
3. Ask: **“Format this for ModCom import.”**
4. Copy the Markdown the AI returns (starts with `## ModCom Incident`).
5. In ModCom: **Incidents → Import from AI** → paste → review → save as AI draft → promote when ready.

Until Import from AI ships, save the Markdown in your incident process and create the record manually — the structure still saves time.

---

## What’s in this kit

| Path | Purpose |
|------|---------|
| [`prompts/01-breach-to-incident.md`](prompts/01-breach-to-incident.md) | **Primary** — monitoring alert / breach analysis → Incident |
| [`prompts/02-audit-finding-to-control-gap.md`](prompts/02-audit-finding-to-control-gap.md) | Future import — publish only for now |
| [`prompts/03-vendor-questionnaire-to-attestation-draft.md`](prompts/03-vendor-questionnaire-to-attestation-draft.md) | Directional — no product import yet |
| [`schemas/incident.markdown.md`](schemas/incident.markdown.md) | Canonical Markdown schema + field map |
| [`schemas/incident.schema.json`](schemas/incident.schema.json) | Thin JSON twin (same fields) |
| [`examples/`](examples/) | Gold-standard sample Incident (MD + JSON) |
| [`POSITIONING.md`](POSITIONING.md) | Behaviour-first messaging (not AI hype) |

---

## Priority & scope

| In scope now | Not yet |
|--------------|---------|
| Incident format + import (product Phase 2) | Control Gap product import |
| Human review / AI draft status | Task auto-create from next steps |
| Any model (Claude, Grok, Cursor, …) | Browser extension / MCP write tools |
| | Email forward |

---

## Rules for AI-generated records

1. Always label as **AI-generated draft — awaiting review**.
2. Do **not** invent facts; use “Unknown — requires human review” when the source is silent.
3. A human must review and promote before the incident is live operationally.
4. Keep provenance (model/tool, reviewer, timestamps) for audit credibility.

---

## Version

- **schema_version:** `1.0`
- **record_type (primary):** `incident`
- **Kit status:** public draft for Week-1 adoption; product paste-import follows Phase 2

Questions: Instilligent / Modular Compliance product docs.
