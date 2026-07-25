---
api_specs:
- filename: bank-first-banking-account-balances-api-openapi.yml
  format: yaml
  label: Bank First Banking Account Balances API
  slug: bank-first-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-banking-account-balances-api-openapi.yml
- filename: bank-first-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Bank First Banking Account Direct Debits API
  slug: bank-first-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-banking-account-direct-debits-api-openapi.yml
- filename: bank-first-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Bank First Banking Account Scheduled Payments API
  slug: bank-first-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-banking-account-scheduled-payments-api-openapi.yml
- filename: bank-first-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Bank First Banking Account Transactions API
  slug: bank-first-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-banking-account-transactions-api-openapi.yml
- filename: bank-first-banking-accounts-api-openapi.yml
  format: yaml
  label: Bank First Banking Accounts API
  slug: bank-first-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-banking-accounts-api-openapi.yml
- filename: bank-first-banking-payees-api-openapi.yml
  format: yaml
  label: Bank First Banking Payees API
  slug: bank-first-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-banking-payees-api-openapi.yml
- filename: bank-first-banking-products-api-openapi.yml
  format: yaml
  label: Bank First Banking Products API
  slug: bank-first-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-banking-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bankfirst.com.au
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: www.bankfirst.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: public.cdr.bankfirst.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bank First Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bank First, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bank First
provider_slug: bank-first
slug: bank-first-domain-security
source_filename: bank-first-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bankfirst.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: false\n- host: public.cdr.bankfirst.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bankfirst.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/security/bank-first-domain-security.yml
summary_line: TLSv1.3 · DMARC
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
