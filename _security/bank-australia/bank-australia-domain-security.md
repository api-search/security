---
api_specs:
- filename: bank-australia-banking-account-balances-api-openapi.yml
  format: yaml
  label: Bank Australia Banking Account Balances API
  slug: bank-australia-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-banking-account-balances-api-openapi.yml
- filename: bank-australia-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Bank Australia Banking Account Direct Debits API
  slug: bank-australia-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-banking-account-direct-debits-api-openapi.yml
- filename: bank-australia-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Bank Australia Banking Account Scheduled Payments API
  slug: bank-australia-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-banking-account-scheduled-payments-api-openapi.yml
- filename: bank-australia-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Bank Australia Banking Account Transactions API
  slug: bank-australia-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-banking-account-transactions-api-openapi.yml
- filename: bank-australia-banking-accounts-api-openapi.yml
  format: yaml
  label: Bank Australia Banking Accounts API
  slug: bank-australia-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-banking-accounts-api-openapi.yml
- filename: bank-australia-banking-payees-api-openapi.yml
  format: yaml
  label: Bank Australia Banking Payees API
  slug: bank-australia-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-banking-payees-api-openapi.yml
- filename: bank-australia-banking-products-api-openapi.yml
  format: yaml
  label: Bank Australia Banking Products API
  slug: bank-australia-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-banking-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bankaust.com.au
  spf: true
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: www.bankaust.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: public.cdr.bankaust.com.au
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bank Australia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bank Australia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bank Australia
provider_slug: bank-australia
slug: bank-australia-domain-security
source_filename: bank-australia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bankaust.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.cdr.bankaust.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\ndomains:\n- domain: bankaust.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/security/bank-australia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Mutual Bank
---
