---
api_specs:
- filename: mcpifex-openapi-generated.yml
  format: yaml
  label: Amdose API
  slug: mcpifex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcpifex/refs/heads/main/openapi/_ae-authored/mcpifex-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mcpifex.com
  spf: false
hosts:
- cert_expires: Jan 15 19:49:12 2027 GMT
  host: mcpifex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mcpifex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amdose, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Amdose
provider_slug: mcpifex
slug: mcpifex-domain-security
source_filename: mcpifex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcpifex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 19:49:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mcpifex.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcpifex/refs/heads/main/security/mcpifex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- MCP
- Marketplace
- AI-Agents
- Integration
---
