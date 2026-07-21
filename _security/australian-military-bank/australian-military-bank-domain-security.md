---
api_specs:
- filename: australian-military-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Australian Military Bank CDR Product Reference Data API
  slug: australian-military-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/openapi/australian-military-bank-cds-banking-products-openapi.yml
- filename: australian-military-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Australian Military Bank CDR Accounts & Balances API
  slug: australian-military-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/openapi/australian-military-bank-cds-banking-products-openapi.yml
- filename: australian-military-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Australian Military Bank CDR Transactions API
  slug: australian-military-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/openapi/australian-military-bank-cds-banking-products-openapi.yml
- filename: australian-military-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Australian Military Bank CDR Direct Debits & Scheduled Payments API
  slug: australian-military-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/openapi/australian-military-bank-cds-banking-products-openapi.yml
- filename: australian-military-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Australian Military Bank CDR Payees API
  slug: australian-military-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/openapi/australian-military-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "microsoft.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: australianmilitarybank.com.au
  spf: true
hosts:
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: www.australianmilitarybank.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: public.open.australianmilitarybank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Australian Military Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Australian Military Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Australian Military Bank
provider_slug: australian-military-bank
slug: australian-military-bank-domain-security
source_filename: australian-military-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.australianmilitarybank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.open.australianmilitarybank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: australianmilitarybank.com.au\n  dnssec: true\n  caa:\n  - 0 issue \"microsoft.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/security/australian-military-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Mutual
- Defence
---
