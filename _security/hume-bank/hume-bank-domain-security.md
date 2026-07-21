---
api_specs:
- filename: hume-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Hume Bank CDR Product Reference Data API
  slug: hume-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-bank/refs/heads/main/openapi/hume-bank-cds-banking-products-openapi.yml
- filename: hume-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Hume Bank CDR Accounts & Balances API
  slug: hume-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-bank/refs/heads/main/openapi/hume-bank-cds-banking-products-openapi.yml
- filename: hume-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Hume Bank CDR Transactions API
  slug: hume-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-bank/refs/heads/main/openapi/hume-bank-cds-banking-products-openapi.yml
- filename: hume-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Hume Bank CDR Direct Debits & Scheduled Payments API
  slug: hume-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-bank/refs/heads/main/openapi/hume-bank-cds-banking-products-openapi.yml
- filename: hume-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Hume Bank CDR Payees API
  slug: hume-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-bank/refs/heads/main/openapi/hume-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: humebank.com.au
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.humebank.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 06:15:46 2026 GMT
  host: ibankob.humebank.com.au
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hume Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hume Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hume Bank
provider_slug: hume-bank
slug: hume-bank-domain-security
source_filename: hume-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.humebank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ibankob.humebank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 06:15:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: humebank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nnote: OpenAPI servers[] enumerate all ~90 Australian CDR data holders (shared multi-bank\n  spec); only Hume Bank hosts are probed here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hume-bank/refs/heads/main/security/hume-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Mutual
- Product Reference Data
---
