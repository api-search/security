---
api_specs:
- filename: bankvic-cds-banking-products-openapi.yml
  format: yaml
  label: BankVic CDR Product Reference Data API
  slug: bankvic-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-cds-banking-products-openapi.yml
- filename: bankvic-cds-banking-products-openapi.yml
  format: yaml
  label: BankVic CDR Accounts & Balances API
  slug: bankvic-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-cds-banking-products-openapi.yml
- filename: bankvic-cds-banking-products-openapi.yml
  format: yaml
  label: BankVic CDR Transactions API
  slug: bankvic-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-cds-banking-products-openapi.yml
- filename: bankvic-cds-banking-products-openapi.yml
  format: yaml
  label: BankVic CDR Direct Debits & Scheduled Payments API
  slug: bankvic-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-cds-banking-products-openapi.yml
- filename: bankvic-cds-banking-products-openapi.yml
  format: yaml
  label: BankVic CDR Payees API
  slug: bankvic-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bankvic.com.au
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.bankvic.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: ib.bankvic.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bankvic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BankVic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BankVic
provider_slug: bankvic
slug: bankvic-domain-security
source_filename: bankvic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bankvic.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ib.bankvic.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bankvic.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/security/bankvic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
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
