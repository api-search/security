---
api_specs:
- filename: commonwealth-bank-accounts-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Accounts API API
  slug: commonwealth-bank-accounts-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-accounts-api-api-openapi.yml
- filename: commonwealth-bank-balances-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Balances API API
  slug: commonwealth-bank-balances-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-balances-api-api-openapi.yml
- filename: commonwealth-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Account Balances API
  slug: commonwealth-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-account-balances-api-openapi.yml
- filename: commonwealth-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Account Direct Debits API
  slug: commonwealth-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-account-direct-debits-api-openapi.yml
- filename: commonwealth-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Account Scheduled Payments API
  slug: commonwealth-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: commonwealth-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Account Transactions API
  slug: commonwealth-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-account-transactions-api-openapi.yml
- filename: commonwealth-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Accounts API
  slug: commonwealth-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-accounts-api-openapi.yml
- filename: commonwealth-bank-banking-payees-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Payees API
  slug: commonwealth-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-payees-api-openapi.yml
- filename: commonwealth-bank-banking-products-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Products API
  slug: commonwealth-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-products-api-openapi.yml
- filename: commonwealth-bank-customer-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Customer API API
  slug: commonwealth-bank-customer-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-customer-api-api-openapi.yml
- filename: commonwealth-bank-payees-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Payees API API
  slug: commonwealth-bank-payees-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-payees-api-api-openapi.yml
- filename: commonwealth-bank-products-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Products API API
  slug: commonwealth-bank-products-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-products-api-api-openapi.yml
- filename: commonwealth-bank-regular-payments-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Regular Payments API API
  slug: commonwealth-bank-regular-payments-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-regular-payments-api-api-openapi.yml
- filename: commonwealth-bank-transaction-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Transaction API API
  slug: commonwealth-bank-transaction-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-transaction-api-api-openapi.yml
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
