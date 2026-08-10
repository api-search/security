---
api_specs:
- filename: niural-authentication-api-openapi.yml
  format: yaml
  label: Niural Authentication API
  slug: niural-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/niural/refs/heads/main/openapi/niural-authentication-api-openapi.yml
- filename: niural-contracts-api-openapi.yml
  format: yaml
  label: Niural Contracts API
  slug: niural-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/niural/refs/heads/main/openapi/niural-contracts-api-openapi.yml
- filename: niural-invoices-api-openapi.yml
  format: yaml
  label: Niural Invoices API
  slug: niural-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/niural/refs/heads/main/openapi/niural-invoices-api-openapi.yml
- filename: niural-transactions-api-openapi.yml
  format: yaml
  label: Niural Transactions API
  slug: niural-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/niural/refs/heads/main/openapi/niural-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: niural.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: www.niural.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 12:53:16 2026 GMT
  host: docs.niural.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: api-live.niural.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Niural Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Niural, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Niural
provider_slug: niural
slug: niural-domain-security
source_filename: niural-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.niural.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.niural.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 12:53:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-live.niural.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: niural.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/niural/refs/heads/main/security/niural-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payroll
- Human Resources
- Employer of Record
- Contractor Management
- Global Payments
- Invoicing
- Compliance
- Fintech
---
