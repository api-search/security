---
api_specs:
- filename: up-bank-accounts-api-openapi.yml
  format: yaml
  label: Up Accounts API
  slug: up-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-accounts-api-openapi.yml
- filename: up-bank-attachments-api-openapi.yml
  format: yaml
  label: Up Attachments API
  slug: up-bank-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-attachments-api-openapi.yml
- filename: up-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: Up Banking Account Balances API
  slug: up-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-banking-account-balances-api-openapi.yml
- filename: up-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Up Banking Account Direct Debits API
  slug: up-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-banking-account-direct-debits-api-openapi.yml
- filename: up-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Up Banking Account Scheduled Payments API
  slug: up-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: up-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Up Banking Account Transactions API
  slug: up-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-banking-account-transactions-api-openapi.yml
- filename: up-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: Up Banking Accounts API
  slug: up-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-banking-accounts-api-openapi.yml
- filename: up-bank-banking-payees-api-openapi.yml
  format: yaml
  label: Up Banking Payees API
  slug: up-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-banking-payees-api-openapi.yml
- filename: up-bank-banking-products-api-openapi.yml
  format: yaml
  label: Up Banking Products API
  slug: up-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-banking-products-api-openapi.yml
- filename: up-bank-categories-api-openapi.yml
  format: yaml
  label: Up Categories API
  slug: up-bank-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-categories-api-openapi.yml
- filename: up-bank-tags-api-openapi.yml
  format: yaml
  label: Up Tags API
  slug: up-bank-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-tags-api-openapi.yml
- filename: up-bank-transactions-api-openapi.yml
  format: yaml
  label: Up Transactions API
  slug: up-bank-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-transactions-api-openapi.yml
- filename: up-bank-utility-endpoints-api-openapi.yml
  format: yaml
  label: Up Utility endpoints API
  slug: up-bank-utility-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-utility-endpoints-api-openapi.yml
- filename: up-bank-webhooks-api-openapi.yml
  format: yaml
  label: Up Webhooks API
  slug: up-bank-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-webhooks-api-openapi.yml
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
