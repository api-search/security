---
api_specs:
- filename: commonwealth-bank-cdr-products-openapi.json
  format: json
  label: Commonwealth Bank CDR Product Reference Data API
  slug: cba-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-cdr-products-openapi.json
- filename: commonwealth-bank-cdr-accounts-openapi.json
  format: json
  label: Commonwealth Bank CDR Accounts & Balances API
  slug: cba-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-cdr-accounts-openapi.json
- filename: commonwealth-bank-cdr-transactions-openapi.json
  format: json
  label: Commonwealth Bank CDR Transactions API
  slug: cba-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-cdr-transactions-openapi.json
- filename: commonwealth-bank-cdr-regular-payments-openapi.json
  format: json
  label: Commonwealth Bank CDR Direct Debits & Scheduled Payments API
  slug: cba-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-cdr-regular-payments-openapi.json
- filename: commonwealth-bank-cdr-payees-openapi.json
  format: json
  label: Commonwealth Bank CDR Payees API
  slug: cba-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-cdr-payees-openapi.json
- filename: commonwealth-bank-cdr-customer-openapi.json
  format: json
  label: Commonwealth Bank CDR Customer API
  slug: cba-cdr-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-cdr-customer-openapi.json
- filename: commonwealth-bank-cds-banking-openapi.json
  format: json
  label: Commonwealth Bank CDR Banking API (DSB Consumer Data Standards)
  slug: cba-cds-banking-standard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-cds-banking-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: commbank.com.au
  spf: true
hosts:
- cert_expires: Jul 24 23:59:59 2026 GMT
  host: www.commbank.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Commonwealth Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commonwealth Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Commonwealth Bank
provider_slug: commonwealth-bank
slug: commonwealth-bank-domain-security
source_filename: commonwealth-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.commbank.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: commbank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/security/commonwealth-bank-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Financial
- Banks
- Consumer Banking
- Business Banking
- Open Banking
- CDR
- Product Reference Data
- ADI
- Australia
---
