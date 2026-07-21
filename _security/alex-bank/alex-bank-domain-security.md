---
api_specs:
- filename: alex-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Alex Bank CDR Product Reference Data API
  slug: alex-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/openapi/alex-bank-cds-banking-products-openapi.yml
- filename: alex-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Alex Bank CDR Accounts & Balances API
  slug: alex-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/openapi/alex-bank-cds-banking-products-openapi.yml
- filename: alex-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Alex Bank CDR Transactions API
  slug: alex-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/openapi/alex-bank-cds-banking-products-openapi.yml
- filename: alex-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Alex Bank CDR Direct Debits & Scheduled Payments API
  slug: alex-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/openapi/alex-bank-cds-banking-products-openapi.yml
- filename: alex-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Alex Bank CDR Payees API
  slug: alex-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/openapi/alex-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: alex.bank
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alex.com.au
  spf: true
hosts:
- cert_expires: Sep 14 07:16:58 2026 GMT
  host: www.alex.bank
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 06:03:10 2026 GMT
  host: public.cdr.alex.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alex Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alex Bank, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Alex Bank
provider_slug: alex-bank
slug: alex-bank-domain-security
source_filename: alex-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alex.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:16:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.cdr.alex.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 06:03:10 2026 GMT\n  hsts: null\ndomains:\n- domain: alex.bank\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: alex.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/security/alex-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Digital Bank
- Product Reference Data
---
