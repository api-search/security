---
api_specs:
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Product Reference Data API
  slug: avenue-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Accounts & Balances API
  slug: avenue-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Transactions API
  slug: avenue-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Direct Debits & Scheduled Payments API
  slug: avenue-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Payees API
  slug: avenue-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: avenuebank.com.au
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.avenuebank.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.avenuebank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avenue Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avenue Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Avenue Bank
provider_slug: avenue-bank
slug: avenue-bank-domain-security
source_filename: avenue-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avenuebank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.avenuebank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: avenuebank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/security/avenue-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Business Banking
- Bank Guarantees
- Australia
- ADI
---
