---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tarx.com
  spf: true
hosts:
- cert_expires: Nov  6 05:11:39 2026 GMT
  host: tarx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  8 06:58:20 2026 GMT
  host: howdy.tarx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  7 05:28:43 2026 GMT
  host: mcp.tarx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Tarx Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TARXAN Inc, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: TARXAN Inc
provider_slug: tarx-com
slug: tarx-com-domain-security
source_filename: tarx-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tarx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  6 05:11:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: howdy.tarx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  8 06:58:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.tarx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 05:28:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tarx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tarx-com/refs/heads/main/security/tarx-com-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI Agents
- Agent Runtime
- Local-First AI
- Private AI
- MCP
- A2A
- LLM
- Inference
- Developer Tools
- Hardware
- Robotics
---
