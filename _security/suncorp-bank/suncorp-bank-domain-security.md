---
api_specs:
- filename: suncorp-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: Suncorp Bank Banking Account Balances API
  slug: suncorp-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-banking-account-balances-api-openapi.yml
- filename: suncorp-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Suncorp Bank Banking Account Direct Debits API
  slug: suncorp-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-banking-account-direct-debits-api-openapi.yml
- filename: suncorp-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Suncorp Bank Banking Account Scheduled Payments API
  slug: suncorp-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: suncorp-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Suncorp Bank Banking Account Transactions API
  slug: suncorp-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-banking-account-transactions-api-openapi.yml
- filename: suncorp-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: Suncorp Bank Banking Accounts API
  slug: suncorp-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-banking-accounts-api-openapi.yml
- filename: suncorp-bank-banking-payees-api-openapi.yml
  format: yaml
  label: Suncorp Bank Banking Payees API
  slug: suncorp-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-banking-payees-api-openapi.yml
- filename: suncorp-bank-banking-products-api-openapi.yml
  format: yaml
  label: Suncorp Bank Banking Products API
  slug: suncorp-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-banking-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: suncorpbank.com.au
  spf: true
hosts:
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: www.suncorpbank.com.au
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: id-ob.suncorpbank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Suncorp Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Suncorp Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Suncorp Bank
provider_slug: suncorp-bank
slug: suncorp-bank-domain-security
source_filename: suncorp-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.suncorpbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: id-ob.suncorpbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: suncorpbank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/security/suncorp-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- Consumer Data Right
---
