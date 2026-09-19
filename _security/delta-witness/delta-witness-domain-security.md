---
api_specs:
- filename: delta-witness-browser-verification-api-openapi.yml
  format: yaml
  label: DELTA Witness — Trust Layer for Autonomous Actions browser verification API
  slug: delta-witness-browser-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-witness/refs/heads/main/openapi/delta-witness-browser-verification-api-openapi.yml
- filename: delta-witness-capture-api-openapi.yml
  format: yaml
  label: DELTA Witness — Trust Layer for Autonomous Actions Capture API
  slug: delta-witness-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-witness/refs/heads/main/openapi/delta-witness-capture-api-openapi.yml
- filename: delta-witness-demo-api-openapi.yml
  format: yaml
  label: DELTA Witness — Trust Layer for Autonomous Actions Demo API
  slug: delta-witness-demo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-witness/refs/heads/main/openapi/delta-witness-demo-api-openapi.yml
- filename: delta-witness-guarded-action-pilot-api-openapi.yml
  format: yaml
  label: DELTA Witness — Trust Layer for Autonomous Actions Guarded Action Pilot API
  slug: delta-witness-guarded-action-pilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-witness/refs/heads/main/openapi/delta-witness-guarded-action-pilot-api-openapi.yml
- filename: delta-witness-health-api-openapi.yml
  format: yaml
  label: DELTA Witness — Trust Layer for Autonomous Actions Health API
  slug: delta-witness-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-witness/refs/heads/main/openapi/delta-witness-health-api-openapi.yml
- filename: delta-witness-preflight-api-openapi.yml
  format: yaml
  label: DELTA Witness — Trust Layer for Autonomous Actions Preflight API
  slug: delta-witness-preflight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-witness/refs/heads/main/openapi/delta-witness-preflight-api-openapi.yml
- filename: delta-witness-preflight-autonomous-action-api-openapi.yml
  format: yaml
  label: DELTA Witness — Trust Layer for Autonomous Actions preflight autonomous action API
  slug: delta-witness-preflight-autonomous-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-witness/refs/heads/main/openapi/delta-witness-preflight-autonomous-action-api-openapi.yml
- filename: delta-witness-proofs-api-openapi.yml
  format: yaml
  label: DELTA Witness — Trust Layer for Autonomous Actions Proofs API
  slug: delta-witness-proofs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-witness/refs/heads/main/openapi/delta-witness-proofs-api-openapi.yml
- filename: delta-witness-quote-api-openapi.yml
  format: yaml
  label: DELTA Witness — Trust Layer for Autonomous Actions Quote API
  slug: delta-witness-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-witness/refs/heads/main/openapi/delta-witness-quote-api-openapi.yml
- filename: delta-witness-watch-api-openapi.yml
  format: yaml
  label: DELTA Witness — Trust Layer for Autonomous Actions Watch API
  slug: delta-witness-watch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-witness/refs/heads/main/openapi/delta-witness-watch-api-openapi.yml
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
- Pay-Per-Use
- base-usdc
- Autonomous Agents
- MCP
- A2A
- Agent Skills
- Trust and Safety
---
