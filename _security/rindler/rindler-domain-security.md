---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: rindler.ai
  spf: true
hosts:
- cert_expires: Sep  9 02:14:44 2026 GMT
  host: rindler.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 17:08:11 2026 GMT
  host: mcp.rindler.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rindler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rindler, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Rindler
provider_slug: rindler
slug: rindler-domain-security
source_filename: rindler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rindler.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 02:14:44 2026 GMT\n  hsts: false\n- host: mcp.rindler.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 17:08:11 2026 GMT\n  hsts: null\ndomains:\n- domain: rindler.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rindler/refs/heads/main/security/rindler-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- MCP
- Model Context Protocol
- AI Agents
- Web Automation
- Browser Automation
- Structured Data
- Website to API
- Agent Tools
- Y Combinator
---
