---
api_specs:
- filename: unity-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: Unity Bank Banking Account Balances API
  slug: unity-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-banking-account-balances-api-openapi.yml
- filename: unity-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Unity Bank Banking Account Direct Debits API
  slug: unity-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-banking-account-direct-debits-api-openapi.yml
- filename: unity-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Unity Bank Banking Account Scheduled Payments API
  slug: unity-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: unity-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Unity Bank Banking Account Transactions API
  slug: unity-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-banking-account-transactions-api-openapi.yml
- filename: unity-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: Unity Bank Banking Accounts API
  slug: unity-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-banking-accounts-api-openapi.yml
- filename: unity-bank-banking-payees-api-openapi.yml
  format: yaml
  label: Unity Bank Banking Payees API
  slug: unity-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-banking-payees-api-openapi.yml
- filename: unity-bank-banking-products-api-openapi.yml
  format: yaml
  label: Unity Bank Banking Products API
  slug: unity-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-banking-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unitybank.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gcmutualbank.com.au
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: www.unitybank.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: ibank.gcmutualbank.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unity Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unity Bank, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Unity Bank
provider_slug: unity-bank
slug: unity-bank-domain-security
source_filename: unity-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unitybank.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ibank.gcmutualbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: unitybank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gcmutualbank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/security/unity-bank-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Mutual Bank
- Product Reference Data
---
