---
api_specs:
- filename: bank-of-us-banking-account-balances-api-openapi.yml
  format: yaml
  label: Bank of us Banking Account Balances API
  slug: bank-of-us-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-banking-account-balances-api-openapi.yml
- filename: bank-of-us-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Bank of us Banking Account Direct Debits API
  slug: bank-of-us-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-banking-account-direct-debits-api-openapi.yml
- filename: bank-of-us-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Bank of us Banking Account Scheduled Payments API
  slug: bank-of-us-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-banking-account-scheduled-payments-api-openapi.yml
- filename: bank-of-us-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Bank of us Banking Account Transactions API
  slug: bank-of-us-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-banking-account-transactions-api-openapi.yml
- filename: bank-of-us-banking-accounts-api-openapi.yml
  format: yaml
  label: Bank of us Banking Accounts API
  slug: bank-of-us-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-banking-accounts-api-openapi.yml
- filename: bank-of-us-banking-payees-api-openapi.yml
  format: yaml
  label: Bank of us Banking Payees API
  slug: bank-of-us-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-banking-payees-api-openapi.yml
- filename: bank-of-us-banking-products-api-openapi.yml
  format: yaml
  label: Bank of us Banking Products API
  slug: bank-of-us-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-banking-products-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bankofus.com.au
  spf: true
hosts:
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: www.bankofus.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.bankofus.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bank Of Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bank of us, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bank of us
provider_slug: bank-of-us
slug: bank-of-us-domain-security
source_filename: bank-of-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bankofus.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bankofus.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bankofus.com.au\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/security/bank-of-us-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Tasmania
- Mutual
- Product Reference Data
---
