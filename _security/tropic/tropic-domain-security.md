---
api_specs:
- filename: tropic-openapi.yml
  format: yaml
  label: Tropic API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tropic/refs/heads/main/openapi/tropic-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tropicapp.io
  spf: true
hosts:
- cert_expires: Aug 16 11:32:13 2026 GMT
  host: www.tropicapp.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:49:32 2026 GMT
  host: help.tropicapp.io
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- host: api.tropicapp.io
  https: false
kind: domain-security
layout: security
method: probed
name: Tropic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tropic, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tropic
provider_slug: tropic
slug: tropic-domain-security
source_filename: tropic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tropicapp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 11:32:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.tropicapp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:49:32 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.tropicapp.io\n  https: false\ndomains:\n- domain: tropicapp.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tropic/refs/heads/main/security/tropic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Benchmarking
- Contract Management
- Cost Optimization
- Procurement
- Renewals
- SaaS Management
- SaaS Procurement
- Spend Management
- Supplier Management
---
