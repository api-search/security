---
api_specs:
- filename: defence-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: Defence Bank Banking Account Balances API
  slug: defence-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-banking-account-balances-api-openapi.yml
- filename: defence-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Defence Bank Banking Account Direct Debits API
  slug: defence-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-banking-account-direct-debits-api-openapi.yml
- filename: defence-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Defence Bank Banking Account Scheduled Payments API
  slug: defence-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: defence-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Defence Bank Banking Account Transactions API
  slug: defence-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-banking-account-transactions-api-openapi.yml
- filename: defence-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: Defence Bank Banking Accounts API
  slug: defence-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-banking-accounts-api-openapi.yml
- filename: defence-bank-banking-payees-api-openapi.yml
  format: yaml
  label: Defence Bank Banking Payees API
  slug: defence-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-banking-payees-api-openapi.yml
- filename: defence-bank-banking-products-api-openapi.yml
  format: yaml
  label: Defence Bank Banking Products API
  slug: defence-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-banking-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: defencebank.com.au
  spf: true
hosts:
- cert_expires: Sep 25 15:23:45 2026 GMT
  host: www.defencebank.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: product.defencebank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Defence Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defence Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Defence Bank
provider_slug: defence-bank
slug: defence-bank-domain-security
source_filename: defence-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.defencebank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 15:23:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: product.defencebank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: defencebank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/security/defence-bank-domain-security.yml
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
