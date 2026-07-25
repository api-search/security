---
api_specs:
- filename: bankvic-banking-account-balances-api-openapi.yml
  format: yaml
  label: BankVic Banking Account Balances API
  slug: bankvic-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-banking-account-balances-api-openapi.yml
- filename: bankvic-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: BankVic Banking Account Direct Debits API
  slug: bankvic-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-banking-account-direct-debits-api-openapi.yml
- filename: bankvic-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: BankVic Banking Account Scheduled Payments API
  slug: bankvic-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-banking-account-scheduled-payments-api-openapi.yml
- filename: bankvic-banking-account-transactions-api-openapi.yml
  format: yaml
  label: BankVic Banking Account Transactions API
  slug: bankvic-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-banking-account-transactions-api-openapi.yml
- filename: bankvic-banking-accounts-api-openapi.yml
  format: yaml
  label: BankVic Banking Accounts API
  slug: bankvic-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-banking-accounts-api-openapi.yml
- filename: bankvic-banking-payees-api-openapi.yml
  format: yaml
  label: BankVic Banking Payees API
  slug: bankvic-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-banking-payees-api-openapi.yml
- filename: bankvic-banking-products-api-openapi.yml
  format: yaml
  label: BankVic Banking Products API
  slug: bankvic-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-banking-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bankvic.com.au
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.bankvic.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: ib.bankvic.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bankvic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BankVic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BankVic
provider_slug: bankvic
slug: bankvic-domain-security
source_filename: bankvic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bankvic.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ib.bankvic.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bankvic.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/security/bankvic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
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
