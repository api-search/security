---
api_specs:
- filename: hsbc-australia-cds-banking-products-openapi.yml
  format: yaml
  label: HSBC Bank Australia CDR Product Reference Data API
  slug: hsbc-australia-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-cds-banking-products-openapi.yml
- filename: hsbc-australia-cds-banking-products-openapi.yml
  format: yaml
  label: HSBC Bank Australia CDR Accounts & Balances API
  slug: hsbc-australia-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-cds-banking-products-openapi.yml
- filename: hsbc-australia-cds-banking-products-openapi.yml
  format: yaml
  label: HSBC Bank Australia CDR Transactions API
  slug: hsbc-australia-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-cds-banking-products-openapi.yml
- filename: hsbc-australia-cds-banking-products-openapi.yml
  format: yaml
  label: HSBC Bank Australia CDR Direct Debits & Scheduled Payments API
  slug: hsbc-australia-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-cds-banking-products-openapi.yml
- filename: hsbc-australia-cds-banking-products-openapi.yml
  format: yaml
  label: HSBC Bank Australia CDR Payees API
  slug: hsbc-australia-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hsbc.com.au
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: www.hsbc.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: public.ob.hsbc.com.au
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hsbc Australia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HSBC Bank Australia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HSBC Bank Australia
provider_slug: hsbc-australia
slug: hsbc-australia-domain-security
source_filename: hsbc-australia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hsbc.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.ob.hsbc.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: hsbc.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/security/hsbc-australia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Product Reference Data
---
