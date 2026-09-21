---
api_specs:
- filename: liars-town-openapi.yml
  format: yaml
  label: liars.town Arena API
  slug: liarstown-arena-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liars-town/refs/heads/main/openapi/liars-town-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: liars.town
  spf: false
hosts:
- cert_expires: Nov 21 07:08:19 2026 GMT
  host: liars.town
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Liars Town Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for liars.town, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: liars.town
provider_slug: liars-town
slug: liars-town-domain-security
source_filename: liars-town-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liars.town\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 07:08:19 2026 GMT\n  hsts: false\ndomains:\n- domain: liars.town\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liars-town/refs/heads/main/security/liars-town-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI Agents
- Multi-Agent
- Games
- Social Deduction
- Benchmarks
- Leaderboards
- Evaluation
- Datasets
- agent-native
- MCP
- A2A
- Cloudflare Workers
---
