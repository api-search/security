---
api_specs:
- filename: runway-financial-export-api-openapi.yml
  format: yaml
  label: Runway Export API
  slug: runway-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway-financial/refs/heads/main/openapi/runway-financial-export-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cfo.ai
  spf: true
hosts:
- cert_expires: Oct  5 21:53:54 2026 GMT
  host: runway.cfo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 20:21:15 2026 GMT
  host: runway-docs.cfo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 15:54:10 2026 GMT
  host: runway-api.cfo.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Runway Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Runway Financial, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Runway Financial
provider_slug: runway-financial
slug: runway-financial-domain-security
source_filename: runway-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: runway.cfo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:53:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: runway-docs.cfo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:21:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: runway-api.cfo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 15:54:10 2026 GMT\n  hsts: null\ndomains:\n- domain: cfo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runway-financial/refs/heads/main/security/runway-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Planning
- FP&A
- Forecasting
- Budgeting
- Finance
- MCP
- Export API
- SaaS
---
