---
api_specs:
- filename: harmonic-ai-companies-api-openapi.yml
  format: yaml
  label: Harmonic REST & GraphQL API
  slug: harmonic-rest-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harmonic-ai/refs/heads/main/openapi/harmonic-ai-companies-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: harmonic.ai
  spf: true
hosts:
- cert_expires: Sep 10 06:24:08 2026 GMT
  host: console.harmonic.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 21:20:13 2026 GMT
  host: api.harmonic.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 21:52:45 2026 GMT
  host: support.harmonic.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harmonic Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harmonic.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Harmonic.ai
provider_slug: harmonic-ai
slug: harmonic-ai-domain-security
source_filename: harmonic-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: console.harmonic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:24:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.harmonic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 21:20:13 2026 GMT\n  hsts: null\n- host: support.harmonic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 21:52:45 2026 GMT\n  hsts: false\ndomains:\n- domain: harmonic.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harmonic-ai/refs/heads/main/security/harmonic-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- startup-intelligence
- venture-capital
- company-data
- people-data
- investor-data
- funding-data
- Data Enrichment
- sales-intelligence
- Market Intelligence
- graphql
- MCP
- agent-native
---
