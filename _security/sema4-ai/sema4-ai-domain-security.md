---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sema4.ai
  spf: true
hosts:
- cert_expires: Oct  8 02:55:55 2026 GMT
  host: sema4.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sema4 Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sema4 Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sema4 Ai
provider_slug: sema4-ai
slug: sema4-ai-domain-security
source_filename: sema4-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sema4.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 02:55:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sema4.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sema4-ai/refs/heads/main/security/sema4-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Automation
- MCP
- Enterprise AI
- Actions
- Python
- Developer Tools
---
