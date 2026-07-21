---
api_specs:
- filename: beyond-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Beyond Bank Australia CDR Product Reference Data API
  slug: beyond-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/openapi/beyond-bank-cds-banking-products-openapi.yml
- filename: beyond-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Beyond Bank Australia CDR Accounts & Balances API
  slug: beyond-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/openapi/beyond-bank-cds-banking-products-openapi.yml
- filename: beyond-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Beyond Bank Australia CDR Transactions API
  slug: beyond-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/openapi/beyond-bank-cds-banking-products-openapi.yml
- filename: beyond-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Beyond Bank Australia CDR Direct Debits & Scheduled Payments API
  slug: beyond-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/openapi/beyond-bank-cds-banking-products-openapi.yml
- filename: beyond-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Beyond Bank Australia CDR Payees API
  slug: beyond-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/openapi/beyond-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: beyondbank.com.au
  spf: true
hosts:
- cert_expires: Aug 26 18:13:56 2026 GMT
  host: www.beyondbank.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 01:29:19 2026 GMT
  host: public.cdr.api.beyondbank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beyond Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beyond Bank Australia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Beyond Bank Australia
provider_slug: beyond-bank
slug: beyond-bank-domain-security
source_filename: beyond-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beyondbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 18:13:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.cdr.api.beyondbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 01:29:19 2026 GMT\n  hsts: null\ndomains:\n- domain: beyondbank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/security/beyond-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Customer Owned
- Product Reference Data
---
