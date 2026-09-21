---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: perkoon.com
  spf: true
hosts:
- cert_expires: Nov 29 17:04:34 2026 GMT
  host: perkoon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Perkoon Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perkoon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Perkoon
provider_slug: perkoon-com
slug: perkoon-com-domain-security
source_filename: perkoon-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: perkoon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 17:04:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: perkoon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perkoon-com/refs/heads/main/security/perkoon-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- File Transfer
- P2P
- WebRTC
- AI Agents
- A2A
- MCP
- CLI
- Agent Skills
- Cloud Storage
- Developer Tools
- Lithuania
---
