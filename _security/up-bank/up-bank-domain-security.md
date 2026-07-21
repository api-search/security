---
api_specs:
- filename: up-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up CDR Product Reference Data API
  slug: up-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-cds-banking-products-openapi.yml
- filename: up-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up CDR Accounts & Balances API
  slug: up-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-cds-banking-products-openapi.yml
- filename: up-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up CDR Transactions API
  slug: up-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-cds-banking-products-openapi.yml
- filename: up-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up CDR Direct Debits & Scheduled Payments API
  slug: up-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-cds-banking-products-openapi.yml
- filename: up-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up CDR Payees API
  slug: up-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-cds-banking-products-openapi.yml
- filename: up-bank-openapi.json
  format: json
  label: Up Personal Banking API
  slug: up-personal-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-openapi.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: up.com.au
  spf: true
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: www.up.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 02:37:38 2026 GMT
  host: api.up.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: developer.up.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Up Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Up, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Up
provider_slug: up-bank
slug: up-bank-domain-security
source_filename: up-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.up.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.up.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:37:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.up.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: up.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/security/up-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Neobank
- Product Reference Data
---
