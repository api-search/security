---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: corvera.ai
  spf: true
hosts:
- cert_expires: Aug 23 22:15:05 2026 GMT
  host: corvera.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 19:31:27 2026 GMT
  host: docs.corvera.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 16:55:15 2026 GMT
  host: mcp.corvera.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Corvera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corvera, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Corvera
provider_slug: corvera
slug: corvera-domain-security
source_filename: corvera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corvera.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 22:15:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.corvera.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 19:31:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mcp.corvera.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 16:55:15 2026 GMT\n  hsts: null\ndomains:\n- domain: corvera.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corvera/refs/heads/main/security/corvera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- MCP
- Model Context Protocol
- CPG
- Consumer Packaged Goods
- Retail
- Data
- Context Layer
- AI Agents
- Analytics
- Y Combinator
---
