---
api_specs:
- filename: cable-api-reference-openapi-original.yml
  format: yaml
  label: Cable API Reference (v2)
  slug: cable-api-reference-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-api-reference-openapi-original.yml
- filename: cable-transaction-data-api-openapi-original.yml
  format: yaml
  label: Cable Transaction Data API
  slug: cable-transaction-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-transaction-data-api-openapi-original.yml
- filename: cable-customer-data-api-openapi-original.yml
  format: yaml
  label: Cable Customer Data API (v1)
  slug: cable-customer-data-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-customer-data-api-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cable.tech
  spf: true
hosts:
- cert_expires: Oct 10 05:29:50 2026 GMT
  host: cable.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 06:56:42 2026 GMT
  host: docs.cable.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:29:37 2026 GMT
  host: api.cable.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Cable
provider_slug: cable
slug: cable-domain-security
source_filename: cable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cable.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 05:29:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cable.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 06:56:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cable.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:29:37 2026 GMT\n  hsts: null\ndomains:\n- domain: cable.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/security/cable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Compliance
- Financial Crime
- RegTech
- Anti-Money Laundering
- Transaction Monitoring
- Screening
- Risk Assessment
- Banking
- Fintech
---
