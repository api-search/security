---
api_specs:
- filename: eqbuilder-dev-openapi.yml
  format: yaml
  label: EQ Scoring Platform API
  slug: eq-scoring-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eqbuilder-dev/refs/heads/main/openapi/eqbuilder-dev-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eqbuilder.dev
  spf: false
hosts:
- cert_expires: Oct 31 23:22:32 2026 GMT
  host: eqbuilder.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eqbuilder Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marz Greta-Lock Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Marz Greta-Lock Network
provider_slug: eqbuilder-dev
slug: eqbuilder-dev-domain-security
source_filename: eqbuilder-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eqbuilder.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:22:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eqbuilder.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eqbuilder-dev/refs/heads/main/security/eqbuilder-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Agent Evaluation
- Benchmarking
- Text Analysis
- Emotional Intelligence
- Conversational AI
- x402
- Agent Payments
- MCP
- A2A
- Developer Tools
---
