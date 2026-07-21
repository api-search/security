---
api_specs:
- filename: regional-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Regional Australia Bank CDR Product Reference Data API
  slug: regional-australia-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/openapi/regional-australia-bank-cds-banking-products-openapi.yml
- filename: regional-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Regional Australia Bank CDR Accounts & Balances API
  slug: regional-australia-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/openapi/regional-australia-bank-cds-banking-products-openapi.yml
- filename: regional-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Regional Australia Bank CDR Transactions API
  slug: regional-australia-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/openapi/regional-australia-bank-cds-banking-products-openapi.yml
- filename: regional-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Regional Australia Bank CDR Direct Debits & Scheduled Payments API
  slug: regional-australia-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/openapi/regional-australia-bank-cds-banking-products-openapi.yml
- filename: regional-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Regional Australia Bank CDR Payees API
  slug: regional-australia-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/openapi/regional-australia-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: regionalaustraliabank.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: regaustbank.io
  spf: true
hosts:
- cert_expires: Aug 23 14:18:14 2026 GMT
  host: www.regionalaustraliabank.com.au
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:46:13 2026 GMT
  host: dashboard.cdr.regionalaustraliabank.com.au
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 04:43:00 2026 GMT
  host: public-data.cdr.regaustbank.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Regional Australia Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Regional Australia Bank, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Regional Australia Bank
provider_slug: regional-australia-bank
slug: regional-australia-bank-domain-security
source_filename: regional-australia-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.regionalaustraliabank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 14:18:14 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: dashboard.cdr.regionalaustraliabank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:46:13 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: public-data.cdr.regaustbank.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 04:43:00 2026 GMT\n  hsts: null\ndomains:\n- domain: regionalaustraliabank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: regaustbank.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/security/regional-australia-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Customer-Owned
- Product Reference Data
- Mutual Bank
---
