---
api_specs:
- filename: dottxt-platform-openapi.yml
  format: yaml
  label: dottxt Platform API
  slug: dottxt-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dottxt/refs/heads/main/openapi/dottxt-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dottxt.ai
  spf: true
hosts:
- cert_expires: Oct  4 14:31:54 2026 GMT
  host: api.dottxt.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dottxt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dottxt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: dottxt
provider_slug: dottxt
slug: dottxt-domain-security
source_filename: dottxt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.dottxt.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:31:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dottxt.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dottxt/refs/heads/main/security/dottxt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- LLM
- Structured Outputs
- JSON Schema
- Machine Learning
- Developer Tools
- Constrained Decoding
---
