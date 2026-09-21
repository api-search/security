---
api_specs:
- filename: theloopbreaker-com-openapi.yml
  format: yaml
  label: Vaultfire Agent Hub API
  slug: vaultfire-agent-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theloopbreaker-com/refs/heads/main/openapi/theloopbreaker-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: theloopbreaker.com
  spf: false
hosts:
- cert_expires: Nov 15 12:40:27 2026 GMT
  host: theloopbreaker.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Theloopbreaker Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vaultfire Protocol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Vaultfire Protocol
provider_slug: theloopbreaker-com
slug: theloopbreaker-com-domain-security
source_filename: theloopbreaker-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theloopbreaker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 12:40:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: theloopbreaker.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theloopbreaker-com/refs/heads/main/security/theloopbreaker-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI Agents
- Agent Identity
- Trust
- Reputation
- Blockchain
- Web3
- Payments
- x402
- MCP
- A2A
- Company
---
