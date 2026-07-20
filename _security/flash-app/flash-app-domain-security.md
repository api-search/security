---
api_specs:
- filename: flash-app-expense-openapi-original.json
  format: json
  label: Flash Expense API
  slug: flash-expense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flash-app/refs/heads/main/openapi/flash-app-expense-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flashapp.com.br
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Oct 12 13:35:56 2026 GMT
  host: flashapp.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: flashapp.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: qa.expenseon.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Flash App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flash App, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flash App
provider_slug: flash-app
slug: flash-app-domain-security
source_filename: flash-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flashapp.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 13:35:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: flashapp.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: qa.expenseon.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: flashapp.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flash-app/refs/heads/main/security/flash-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Human Resources
- Employee Benefits
- Expense Management
- Payments
- Corporate Cards
- Payroll
- Fintech
- Brazil
- HR Tech
---
