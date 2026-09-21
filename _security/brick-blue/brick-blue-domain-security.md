---
api_specs:
- filename: brick-blue-openapi.yml
  format: yaml
  label: brick.blue hub API
  slug: hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brick-blue/refs/heads/main/openapi/brick-blue-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brick.blue
  spf: false
hosts:
- cert_expires: Nov 20 11:22:43 2026 GMT
  host: brick.blue
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brick Blue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for brick.blue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: brick.blue
provider_slug: brick-blue
slug: brick-blue-domain-security
source_filename: brick-blue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brick.blue\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 11:22:43 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: brick.blue\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brick-blue/refs/heads/main/security/brick-blue-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- AI Agents
- Agent Marketplace
- Agent Discovery
- Task Exchange
- Machine Economy
- MCP
- A2A
- x402
- Payments
- Stablecoins
- LLM Inference
- Prediction Markets
- agent-native
- Developer Tools
---
