---
api_specs:
- filename: mystate-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: MyState Bank Banking Account Balances API
  slug: mystate-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystate-bank/refs/heads/main/openapi/mystate-bank-banking-account-balances-api-openapi.yml
- filename: mystate-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: MyState Bank Banking Account Direct Debits API
  slug: mystate-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystate-bank/refs/heads/main/openapi/mystate-bank-banking-account-direct-debits-api-openapi.yml
- filename: mystate-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: MyState Bank Banking Account Scheduled Payments API
  slug: mystate-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystate-bank/refs/heads/main/openapi/mystate-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: mystate-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: MyState Bank Banking Account Transactions API
  slug: mystate-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystate-bank/refs/heads/main/openapi/mystate-bank-banking-account-transactions-api-openapi.yml
- filename: mystate-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: MyState Bank Banking Accounts API
  slug: mystate-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystate-bank/refs/heads/main/openapi/mystate-bank-banking-accounts-api-openapi.yml
- filename: mystate-bank-banking-payees-api-openapi.yml
  format: yaml
  label: MyState Bank Banking Payees API
  slug: mystate-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystate-bank/refs/heads/main/openapi/mystate-bank-banking-payees-api-openapi.yml
- filename: mystate-bank-banking-products-api-openapi.yml
  format: yaml
  label: MyState Bank Banking Products API
  slug: mystate-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystate-bank/refs/heads/main/openapi/mystate-bank-banking-products-api-openapi.yml
- filename: mystate-bank-products-api-openapi.yml
  format: yaml
  label: MyState Bank Products API
  slug: mystate-bank-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystate-bank/refs/heads/main/openapi/mystate-bank-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mystate.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: commbank.com.au
  spf: true
hosts:
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: www.mystate.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: public.cdr.mystate.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: api.commbank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mystate Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyState Bank, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MyState Bank
provider_slug: mystate-bank
slug: mystate-bank-domain-security
source_filename: mystate-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mystate.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.cdr.mystate.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\n- host: api.commbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: mystate.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: commbank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mystate-bank/refs/heads/main/security/mystate-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Product Reference Data
---
