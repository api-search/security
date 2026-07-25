---
api_specs:
- filename: bankwest-banking-account-balances-api-openapi.yml
  format: yaml
  label: Bankwest Banking Account Balances API
  slug: bankwest-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-banking-account-balances-api-openapi.yml
- filename: bankwest-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Bankwest Banking Account Direct Debits API
  slug: bankwest-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-banking-account-direct-debits-api-openapi.yml
- filename: bankwest-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Bankwest Banking Account Scheduled Payments API
  slug: bankwest-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-banking-account-scheduled-payments-api-openapi.yml
- filename: bankwest-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Bankwest Banking Account Transactions API
  slug: bankwest-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-banking-account-transactions-api-openapi.yml
- filename: bankwest-banking-accounts-api-openapi.yml
  format: yaml
  label: Bankwest Banking Accounts API
  slug: bankwest-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-banking-accounts-api-openapi.yml
- filename: bankwest-banking-payees-api-openapi.yml
  format: yaml
  label: Bankwest Banking Payees API
  slug: bankwest-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-banking-payees-api-openapi.yml
- filename: bankwest-banking-products-api-openapi.yml
  format: yaml
  label: Bankwest Banking Products API
  slug: bankwest-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-banking-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bankwest.com.au
  spf: true
hosts:
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: www.bankwest.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: open-api.bankwest.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bankwest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bankwest, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bankwest
provider_slug: bankwest
slug: bankwest-domain-security
source_filename: bankwest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bankwest.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open-api.bankwest.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bankwest.com.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/security/bankwest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- Digital Bank
---
