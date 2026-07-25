---
api_specs:
- filename: people-first-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: People First Bank Banking Account Balances API
  slug: people-first-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-first-bank/refs/heads/main/openapi/people-first-bank-banking-account-balances-api-openapi.yml
- filename: people-first-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: People First Bank Banking Account Direct Debits API
  slug: people-first-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-first-bank/refs/heads/main/openapi/people-first-bank-banking-account-direct-debits-api-openapi.yml
- filename: people-first-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: People First Bank Banking Account Scheduled Payments API
  slug: people-first-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-first-bank/refs/heads/main/openapi/people-first-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: people-first-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: People First Bank Banking Account Transactions API
  slug: people-first-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-first-bank/refs/heads/main/openapi/people-first-bank-banking-account-transactions-api-openapi.yml
- filename: people-first-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: People First Bank Banking Accounts API
  slug: people-first-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-first-bank/refs/heads/main/openapi/people-first-bank-banking-accounts-api-openapi.yml
- filename: people-first-bank-banking-payees-api-openapi.yml
  format: yaml
  label: People First Bank Banking Payees API
  slug: people-first-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-first-bank/refs/heads/main/openapi/people-first-bank-banking-payees-api-openapi.yml
- filename: people-first-bank-banking-products-api-openapi.yml
  format: yaml
  label: People First Bank Banking Products API
  slug: people-first-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-first-bank/refs/heads/main/openapi/people-first-bank-banking-products-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "ssl.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issuewild "ssl.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: peoplefirstbank.com.au
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.peoplefirstbank.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: public.openbanking.peoplefirstbank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: People First Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for People First Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: People First Bank
provider_slug: people-first-bank
slug: people-first-bank-domain-security
source_filename: people-first-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.peoplefirstbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.openbanking.peoplefirstbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: peoplefirstbank.com.au\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/people-first-bank/refs/heads/main/security/people-first-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Mutual Bank
- Product Reference Data
---
