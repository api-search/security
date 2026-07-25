---
api_specs:
- filename: westpac-banking-account-balances-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Account Balances API
  slug: westpac-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-account-balances-api-openapi.yml
- filename: westpac-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Account Direct Debits API
  slug: westpac-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-account-direct-debits-api-openapi.yml
- filename: westpac-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Account Scheduled Payments API
  slug: westpac-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-account-scheduled-payments-api-openapi.yml
- filename: westpac-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Account Transactions API
  slug: westpac-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-account-transactions-api-openapi.yml
- filename: westpac-banking-accounts-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Accounts API
  slug: westpac-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-accounts-api-openapi.yml
- filename: westpac-banking-payees-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Payees API
  slug: westpac-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-payees-api-openapi.yml
- filename: westpac-banking-products-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Products API
  slug: westpac-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-products-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: westpac.com.au
  spf: true
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: www.westpac.com.au
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: digital-api.westpac.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Westpac Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Westpac Banking Corporation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Westpac Banking Corporation
provider_slug: westpac
slug: westpac-domain-security
source_filename: westpac-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.westpac.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: digital-api.westpac.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: westpac.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/security/westpac-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
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
