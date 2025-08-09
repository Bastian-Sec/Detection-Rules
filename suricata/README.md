# Suricata Rules

This folder contains Suricata rules grouped by topic:

- **ip.rules** → IP-based detections.
- **ports.rules** → Suspicious or uncommon ports and services.
- **dns.rules** → Malicious domains or abnormal DNS activity.
- **http.rules** → Suspicious HTTP traffic patterns.

## Conventions
- Same structure as Snort but SIDs start from `2000001`.
- Severity: `low | medium | high | critical`.
- One rule per line for clarity, with comments at the top.

## Example Usage
```bash
suricata -c /etc/suricata/suricata.yaml -r sample.pcap

