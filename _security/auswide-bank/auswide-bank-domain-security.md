---
api_specs:
- filename: auswide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Auswide Bank CDR Product Reference Data API
  slug: auswide-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auswide-bank/refs/heads/main/openapi/auswide-bank-cds-banking-products-openapi.yml
- filename: auswide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Auswide Bank CDR Accounts & Balances API
  slug: auswide-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auswide-bank/refs/heads/main/openapi/auswide-bank-cds-banking-products-openapi.yml
- filename: auswide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Auswide Bank CDR Transactions API
  slug: auswide-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auswide-bank/refs/heads/main/openapi/auswide-bank-cds-banking-products-openapi.yml
- filename: auswide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Auswide Bank CDR Direct Debits & Scheduled Payments API
  slug: auswide-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auswide-bank/refs/heads/main/openapi/auswide-bank-cds-banking-products-openapi.yml
- filename: auswide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Auswide Bank CDR Payees API
  slug: auswide-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auswide-bank/refs/heads/main/openapi/auswide-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: auswidebank.com.au
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.auswidebank.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: api.auswidebank.com.au
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Auswide Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auswide Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Auswide Bank
provider_slug: auswide-bank
slug: auswide-bank-domain-security
source_filename: auswide-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.auswidebank.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.auswidebank.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: auswidebank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auswide-bank/refs/heads/main/security/auswide-bank-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
---
