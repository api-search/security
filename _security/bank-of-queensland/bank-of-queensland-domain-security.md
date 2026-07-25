---
api_specs:
- filename: bank-of-queensland-banking-account-balances-api-openapi.yml
  format: yaml
  label: Bank of Queensland Banking Account Balances API
  slug: bank-of-queensland-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-banking-account-balances-api-openapi.yml
- filename: bank-of-queensland-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Bank of Queensland Banking Account Direct Debits API
  slug: bank-of-queensland-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-banking-account-direct-debits-api-openapi.yml
- filename: bank-of-queensland-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Bank of Queensland Banking Account Scheduled Payments API
  slug: bank-of-queensland-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-banking-account-scheduled-payments-api-openapi.yml
- filename: bank-of-queensland-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Bank of Queensland Banking Account Transactions API
  slug: bank-of-queensland-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-banking-account-transactions-api-openapi.yml
- filename: bank-of-queensland-banking-accounts-api-openapi.yml
  format: yaml
  label: Bank of Queensland Banking Accounts API
  slug: bank-of-queensland-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-banking-accounts-api-openapi.yml
- filename: bank-of-queensland-banking-payees-api-openapi.yml
  format: yaml
  label: Bank of Queensland Banking Payees API
  slug: bank-of-queensland-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-banking-payees-api-openapi.yml
- filename: bank-of-queensland-banking-products-api-openapi.yml
  format: yaml
  label: Bank of Queensland Banking Products API
  slug: bank-of-queensland-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-banking-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: boq.com.au
  spf: true
hosts:
- cert_expires: Aug 16 23:59:59 2026 GMT
  host: www.boq.com.au
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: secure.api.boq.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bank Of Queensland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bank of Queensland, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bank of Queensland
provider_slug: bank-of-queensland
slug: bank-of-queensland-domain-security
source_filename: bank-of-queensland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boq.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: secure.api.boq.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: boq.com.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/security/bank-of-queensland-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
---
