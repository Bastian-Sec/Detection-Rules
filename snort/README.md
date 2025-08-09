# Snort Rules

This folder contains Snort rules grouped by topic:

- **ip.rules** → IP-based detections (malicious hosts, IOC lists).
- **ports.rules** → Suspicious or uncommon ports and services.
- **dns.rules** → Malicious domains, suspicious DNS queries, tunneling detection.
- **http.rules** → Unusual HTTP methods, suspicious user-agents, paths, or headers.

## Naming and Conventions
- File names follow `<topic>.rules`.
- Each rule must include a comment header describing its purpose, topic, severity, and references.
- Use unique SIDs starting from `1000001` for this repository and increment by +1.
- Severity levels: `low | medium | high | critical`.

## Example Usage
To test rules:
```bash
snort -c /path/to/snort.conf -r sample.pcap
