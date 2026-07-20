---
api_specs:
- filename: airweave-openapi.json
  format: json
  label: Airweave API
  slug: airweave-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airweave/refs/heads/main/openapi/airweave-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airweave.ai
  spf: true
hosts:
- cert_expires: Oct 15 18:03:00 2026 GMT
  host: airweave.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 11:15:36 2026 GMT
  host: api.airweave.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airweave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airweave, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Airweave
provider_slug: airweave
slug: airweave-domain-security
source_filename: airweave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airweave.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 18:03:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.airweave.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 11:15:36 2026 GMT\n  hsts: null\ndomains:\n- domain: airweave.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airweave/refs/heads/main/security/airweave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Search
- RAG
- Retrieval
- Agents
- MCP
- Vector Search
- Data Integration
- Context
---
