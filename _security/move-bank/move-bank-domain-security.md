---
api_specs:
- filename: move-bank-cds-banking-products-openapi.yml
  format: yaml
  label: MOVE Bank CDR Product Reference Data API
  slug: move-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-cds-banking-products-openapi.yml
- filename: move-bank-cds-banking-products-openapi.yml
  format: yaml
  label: MOVE Bank CDR Accounts & Balances API
  slug: move-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-cds-banking-products-openapi.yml
- filename: move-bank-cds-banking-products-openapi.yml
  format: yaml
  label: MOVE Bank CDR Transactions API
  slug: move-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-cds-banking-products-openapi.yml
- filename: move-bank-cds-banking-products-openapi.yml
  format: yaml
  label: MOVE Bank CDR Direct Debits & Scheduled Payments API
  slug: move-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-cds-banking-products-openapi.yml
- filename: move-bank-cds-banking-products-openapi.yml
  format: yaml
  label: MOVE Bank CDR Payees API
  slug: move-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: movebank.com.au
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: www.movebank.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: openbanking.movebank.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Move Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MOVE Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MOVE Bank
provider_slug: move-bank
slug: move-bank-domain-security
source_filename: move-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.movebank.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: openbanking.movebank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: movebank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/security/move-bank-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Mutual Bank
- Australia
- Product Reference Data
---
