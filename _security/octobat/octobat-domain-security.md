---
api_specs:
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Invoices API
  slug: octobat-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Credit Notes API
  slug: octobat-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Transactions API
  slug: octobat-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Customers API
  slug: octobat-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Products API
  slug: octobat-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Tax Evidence API
  slug: octobat-tax-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Coupons API
  slug: octobat-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Subscriptions API
  slug: octobat-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Payouts API
  slug: octobat-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: octobat.com
  spf: true
hosts:
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: www.octobat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 06:50:12 2026 GMT
  host: docs.octobat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: apiv2.octobat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Octobat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Octobat, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Octobat
provider_slug: octobat
slug: octobat-domain-security
source_filename: octobat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.octobat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.octobat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 06:50:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apiv2.octobat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: octobat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/security/octobat-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Billing
- Invoicing
- Tax Compliance
- VAT
- E-Commerce
- Payments
- Fintech
---
