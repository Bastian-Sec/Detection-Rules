# Sigma Rules

This folder contains Sigma rules grouped by topic:

- **ip.yml** → Detects events with specific IP addresses.
- **ports.yml** → Detects usage of suspicious ports.
- **dns.yml** → Flags suspicious or malicious domains.
- **http.yml** → Matches HTTP requests with suspicious patterns.

## Conventions
- Sigma rules must be valid YAML.
- Include `title`, `description`, `status`, `level`, `references`, `tags`, `logsource`, and `detection` sections.
- Topics: `IP | Ports | DNS | HTTP`.

## Example Usage
To convert a Sigma rule to Splunk SPL:
```bash
sigmac -t splunk ip.yml

