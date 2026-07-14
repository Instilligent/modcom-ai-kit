# Examples

Gold fixtures for parser tests and human dry-runs.

| File | Format | Scenario |
|------|--------|----------|
| `crushftp-credential-exposure.incident.md` | Markdown | High / security — credential exposure |
| `crushftp-credential-exposure.incident.json` | JSON | Same as above |
| `near-miss-slip-operational.incident.md` | Markdown | Low / operational — warehouse near-miss |
| `near-miss-slip-operational.incident.json` | JSON | Same as above |

Product parsers should accept either format and map to Incident fields with `status = ai_draft`.