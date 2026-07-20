---
api_specs:
- filename: end-close-openapi-original.json
  format: json
  label: End Close API
  slug: end-close-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/openapi/end-close-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: endclose.com
  spf: true
hosts:
- cert_expires: Sep 29 16:49:10 2026 GMT
  host: api.endclose.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: End Close Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for End Close, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: End Close
provider_slug: end-close
slug: end-close-domain-security
source_filename: end-close-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.endclose.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 16:49:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: endclose.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/security/end-close-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Reconciliation
- Payments
- Financial Operations
- Accounting
- Banking
- Data Integration
- Webhooks
- Fintech
---
