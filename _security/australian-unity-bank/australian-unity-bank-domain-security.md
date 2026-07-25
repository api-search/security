---
api_specs:
- filename: australian-unity-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: Australian Unity Bank Banking Account Balances API
  slug: australian-unity-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-banking-account-balances-api-openapi.yml
- filename: australian-unity-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Australian Unity Bank Banking Account Direct Debits API
  slug: australian-unity-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-banking-account-direct-debits-api-openapi.yml
- filename: australian-unity-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Australian Unity Bank Banking Account Scheduled Payments API
  slug: australian-unity-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: australian-unity-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Australian Unity Bank Banking Account Transactions API
  slug: australian-unity-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-banking-account-transactions-api-openapi.yml
- filename: australian-unity-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: Australian Unity Bank Banking Accounts API
  slug: australian-unity-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-banking-accounts-api-openapi.yml
- filename: australian-unity-bank-banking-payees-api-openapi.yml
  format: yaml
  label: Australian Unity Bank Banking Payees API
  slug: australian-unity-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-banking-payees-api-openapi.yml
- filename: australian-unity-bank-banking-products-api-openapi.yml
  format: yaml
  label: Australian Unity Bank Banking Products API
  slug: australian-unity-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-banking-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: australianunity.com.au
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: www.australianunity.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: open-banking.australianunity.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Australian Unity Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Australian Unity Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Australian Unity Bank
provider_slug: australian-unity-bank
slug: australian-unity-bank-domain-security
source_filename: australian-unity-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.australianunity.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open-banking.australianunity.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: australianunity.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/security/australian-unity-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Mutual
- Product Reference Data
---
