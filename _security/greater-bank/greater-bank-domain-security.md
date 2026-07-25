---
api_specs:
- filename: greater-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: Greater Bank Banking Account Balances API
  slug: greater-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greater-bank/refs/heads/main/openapi/greater-bank-banking-account-balances-api-openapi.yml
- filename: greater-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Greater Bank Banking Account Direct Debits API
  slug: greater-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greater-bank/refs/heads/main/openapi/greater-bank-banking-account-direct-debits-api-openapi.yml
- filename: greater-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Greater Bank Banking Account Scheduled Payments API
  slug: greater-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greater-bank/refs/heads/main/openapi/greater-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: greater-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Greater Bank Banking Account Transactions API
  slug: greater-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greater-bank/refs/heads/main/openapi/greater-bank-banking-account-transactions-api-openapi.yml
- filename: greater-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: Greater Bank Banking Accounts API
  slug: greater-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greater-bank/refs/heads/main/openapi/greater-bank-banking-accounts-api-openapi.yml
- filename: greater-bank-banking-payees-api-openapi.yml
  format: yaml
  label: Greater Bank Banking Payees API
  slug: greater-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greater-bank/refs/heads/main/openapi/greater-bank-banking-payees-api-openapi.yml
- filename: greater-bank-banking-products-api-openapi.yml
  format: yaml
  label: Greater Bank Banking Products API
  slug: greater-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greater-bank/refs/heads/main/openapi/greater-bank-banking-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: greater.com.au
  spf: true
hosts:
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: www.greater.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: public.cdr.greater.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Greater Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greater Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Greater Bank
provider_slug: greater-bank
slug: greater-bank-domain-security
source_filename: greater-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.greater.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: null\n- host: public.cdr.greater.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: greater.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greater-bank/refs/heads/main/security/greater-bank-domain-security.yml
summary_line: TLSv1.3 · DMARC
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
