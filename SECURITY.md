# Security

This repository is **prompts and schemas only** — no servers, no database, no auth.

## Product path (Modular Compliance)

When import is enabled in the ModCom product:

- AI-generated records must land as **drafts** until a human with elevate privileges promotes them.
- Mapped fields are sanitized (HTML stripped); raw paste is for audit, not HTML rendering.
- Paste size is limited; tenant identity comes from the authenticated session, not the paste.
- Security four-eyes + pen-test checklist are required before shipping import routes.

## Reporting

For vulnerabilities in the **Modular Compliance product**, contact Instilligent support / security channel.  
Do not file product secrets or production credentials in public issues.

## Related

- Product monorepo: private Instilligent/ModularCompliance  
- Positioning: [POSITIONING.md](./POSITIONING.md)
