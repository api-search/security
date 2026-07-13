---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: roocode.com
  spf: true
hosts:
- cert_expires: Sep 13 04:35:34 2026 GMT
  host: roocode.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 06:52:51 2026 GMT
  host: docs.roocode.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roorules Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for .Roorules, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: .Roorules
provider_slug: roorules
slug: roorules-domain-security
source_filename: roorules-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: roocode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:35:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.roocode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 06:52:51 2026 GMT\n  hsts: false\ndomains:\n- domain: roocode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roorules/refs/heads/main/security/roorules-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- AI Copilot
- Coding Assistant
- Coding Standards
- Developer Workflow
- LLM
- MCP
- Roo Code
- VS Code
---
