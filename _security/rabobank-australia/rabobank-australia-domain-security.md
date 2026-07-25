---
api_specs:
- filename: rabobank-australia-banking-account-balances-api-openapi.yml
  format: yaml
  label: Rabobank Australia Banking Account Balances API
  slug: rabobank-australia-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-banking-account-balances-api-openapi.yml
- filename: rabobank-australia-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Rabobank Australia Banking Account Direct Debits API
  slug: rabobank-australia-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-banking-account-direct-debits-api-openapi.yml
- filename: rabobank-australia-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Rabobank Australia Banking Account Scheduled Payments API
  slug: rabobank-australia-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-banking-account-scheduled-payments-api-openapi.yml
- filename: rabobank-australia-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Rabobank Australia Banking Account Transactions API
  slug: rabobank-australia-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-banking-account-transactions-api-openapi.yml
- filename: rabobank-australia-banking-accounts-api-openapi.yml
  format: yaml
  label: Rabobank Australia Banking Accounts API
  slug: rabobank-australia-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-banking-accounts-api-openapi.yml
- filename: rabobank-australia-banking-payees-api-openapi.yml
  format: yaml
  label: Rabobank Australia Banking Payees API
  slug: rabobank-australia-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-banking-payees-api-openapi.yml
- filename: rabobank-australia-banking-products-api-openapi.yml
  format: yaml
  label: Rabobank Australia Banking Products API
  slug: rabobank-australia-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-banking-products-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "quovadisglobal.com"
  - 0 iodef "mailto:Certificate.Operations@rabobank.com"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rabobank.com.au
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: www.rabobank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: openbanking.api.rabobank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rabobank Australia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rabobank Australia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rabobank Australia
provider_slug: rabobank-australia
slug: rabobank-australia-domain-security
source_filename: rabobank-australia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rabobank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: null\n- host: openbanking.api.rabobank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: rabobank.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"quovadisglobal.com\"\n  - 0 iodef \"mailto:Certificate.Operations@rabobank.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/security/rabobank-australia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Agribusiness
- Product Reference Data
---
