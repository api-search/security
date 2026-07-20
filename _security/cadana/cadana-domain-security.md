---
api_specs:
- filename: cadana-workforce-management-openapi.yaml
  format: yaml
  label: Business Workforce Management
  slug: business-workforce-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadana/refs/heads/main/openapi/cadana-workforce-management-openapi.yaml
- filename: cadana-embedded-payments-openapi.yaml
  format: yaml
  label: Embedded Payments
  slug: embedded-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadana/refs/heads/main/openapi/cadana-embedded-payments-openapi.yaml
- filename: cadana-embedded-consumer-wallets-openapi.yaml
  format: yaml
  label: Embedded Consumer Wallets
  slug: embedded-consumer-wallets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadana/refs/heads/main/openapi/cadana-embedded-consumer-wallets-openapi.yaml
- filename: cadana-global-tax-openapi.yaml
  format: yaml
  label: Global Tax Engine
  slug: global-tax-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadana/refs/heads/main/openapi/cadana-global-tax-openapi.yaml
- filename: cadana-statutory-compliance-openapi.yaml
  format: yaml
  label: Statutory Compliance API
  slug: statutory-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadana/refs/heads/main/openapi/cadana-statutory-compliance-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cadanapay.com
  spf: true
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: cadanapay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: api.cadanapay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: dev-api.cadanapay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cadana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cadana, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cadana
provider_slug: cadana
slug: cadana-domain-security
source_filename: cadana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cadanapay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cadanapay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\n- host: dev-api.cadanapay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cadanapay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cadana/refs/heads/main/security/cadana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payroll
- Payments
- Global Payroll
- Contractor Payments
- Embedded Finance
- Wallets
- Tax
- Compliance
- Fintech
- Money Transfer
- White Label
---
