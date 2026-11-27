---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mcploadbudgeter.space
  spf: false
hosts:
- cert_expires: Dec 26 03:07:24 2026 GMT
  host: mcploadbudgeter.space
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MCPLoad Budgeter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MCPLoad Budgeter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MCPLoad Budgeter
provider_slug: mcploadbudgeter-space
slug: mcploadbudgeter-space-domain-security
source_filename: mcploadbudgeter-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcploadbudgeter.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 03:07:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mcploadbudgeter.space\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mcploadbudgeter-space/security/mcploadbudgeter-space-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Budgeting
- Tools
- MCP
- Optimization
---
