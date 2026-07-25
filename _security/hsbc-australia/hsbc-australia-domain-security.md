---
api_specs:
- filename: hsbc-australia-banking-account-balances-api-openapi.yml
  format: yaml
  label: HSBC Bank Australia Banking Account Balances API
  slug: hsbc-australia-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-banking-account-balances-api-openapi.yml
- filename: hsbc-australia-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: HSBC Bank Australia Banking Account Direct Debits API
  slug: hsbc-australia-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-banking-account-direct-debits-api-openapi.yml
- filename: hsbc-australia-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: HSBC Bank Australia Banking Account Scheduled Payments API
  slug: hsbc-australia-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-banking-account-scheduled-payments-api-openapi.yml
- filename: hsbc-australia-banking-account-transactions-api-openapi.yml
  format: yaml
  label: HSBC Bank Australia Banking Account Transactions API
  slug: hsbc-australia-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-banking-account-transactions-api-openapi.yml
- filename: hsbc-australia-banking-accounts-api-openapi.yml
  format: yaml
  label: HSBC Bank Australia Banking Accounts API
  slug: hsbc-australia-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-banking-accounts-api-openapi.yml
- filename: hsbc-australia-banking-payees-api-openapi.yml
  format: yaml
  label: HSBC Bank Australia Banking Payees API
  slug: hsbc-australia-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-banking-payees-api-openapi.yml
- filename: hsbc-australia-banking-products-api-openapi.yml
  format: yaml
  label: HSBC Bank Australia Banking Products API
  slug: hsbc-australia-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-banking-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hsbc.com.au
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: www.hsbc.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: public.ob.hsbc.com.au
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hsbc Australia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HSBC Bank Australia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HSBC Bank Australia
provider_slug: hsbc-australia
slug: hsbc-australia-domain-security
source_filename: hsbc-australia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hsbc.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.ob.hsbc.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: hsbc.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/security/hsbc-australia-domain-security.yml
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
