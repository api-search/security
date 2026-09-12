---
api_specs:
- filename: openapi.json
  format: json
  label: DELTA Witness API
  slug: delta-witness-api
  spec_type: OpenAPI
  url: https://delta-witness-api.ruphussten.workers.dev/openapi.json
- filename: delta-witness-partner-gateway-openapi.json
  format: json
  label: DELTA Witness Partner Gateway
  slug: delta-witness-partner-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-witness/refs/heads/main/openapi/delta-witness-partner-gateway-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workers.dev
  spf: true
hosts:
- cert_expires: Nov 21 11:24:56 2026 GMT
  host: delta-witness-api.ruphussten.workers.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Delta Witness Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DELTA Witness — Trust Layer for Autonomous Actions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DELTA Witness — Trust Layer for Autonomous Actions
provider_slug: delta-witness
slug: delta-witness-domain-security
source_filename: delta-witness-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: delta-witness-api.ruphussten.workers.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 11:24:56 2026 GMT\n  hsts: false\ndomains:\n- domain: workers.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delta-witness/refs/heads/main/security/delta-witness-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- web-verification
- proof-of-observation
- page-state-monitoring
- content-hashing
- agent-guardrails
- preflight-checks
- x402-payments
- pay-per-use
- base-usdc
- autonomous-agents
- mcp
- a2a
- agent-skill
- trust-and-safety
---
