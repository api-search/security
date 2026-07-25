---
api_specs:
- filename: racq-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: RACQ Bank Banking Account Balances API
  slug: racq-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-banking-account-balances-api-openapi.yml
- filename: racq-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: RACQ Bank Banking Account Direct Debits API
  slug: racq-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-banking-account-direct-debits-api-openapi.yml
- filename: racq-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: RACQ Bank Banking Account Scheduled Payments API
  slug: racq-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: racq-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: RACQ Bank Banking Account Transactions API
  slug: racq-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-banking-account-transactions-api-openapi.yml
- filename: racq-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: RACQ Bank Banking Accounts API
  slug: racq-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-banking-accounts-api-openapi.yml
- filename: racq-bank-banking-payees-api-openapi.yml
  format: yaml
  label: RACQ Bank Banking Payees API
  slug: racq-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-banking-payees-api-openapi.yml
- filename: racq-bank-banking-products-api-openapi.yml
  format: yaml
  label: RACQ Bank Banking Products API
  slug: racq-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-banking-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: racq.com.au
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.racq.com.au
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: cdrbank.racq.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Racq Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RACQ Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RACQ Bank
provider_slug: racq-bank
slug: racq-bank-domain-security
source_filename: racq-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.racq.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: cdrbank.racq.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: racq.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/security/racq-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
- Mutual
---
