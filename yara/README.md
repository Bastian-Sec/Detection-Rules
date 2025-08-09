# YARA Rules

This folder contains YARA rules grouped by topic:

- **ip.yar** → Detects hardcoded IPs or IP patterns.
- **ports.yar** → Detects specific port numbers in binaries or configs.
- **dns.yar** → Matches suspicious domain names.
- **http.yar** → Detects suspicious HTTP strings or user-agents.

## Conventions
- All rules must include a `meta` section with `name`, `topic`, `severity`, `refs`, `author`, and `date`.
- Keep descriptions short but precise.
- Severity: `low | medium | high | critical`.

## Example Usage
```bash
yara -r ip.yar /path/to/scan

