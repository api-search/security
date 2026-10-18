---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mcpforge.tech
  spf: true
hosts:
- cert_expires: Dec 19 22:33:30 2026 GMT
  host: mcpforge.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mcpforge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MCPForge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MCPForge
provider_slug: mcpforge
slug: mcpforge-domain-security
source_filename: mcpforge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcpforge.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 22:33:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mcpforge.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcpforge/refs/heads/main/security/mcpforge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- MCP
- Verification
- Security
- API
- Platform
---
