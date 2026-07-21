---
api_specs:
- filename: qudos-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Qudos Bank CDR Product Reference Data API
  slug: qudos-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/openapi/qudos-bank-cds-banking-products-openapi.yml
- filename: qudos-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Qudos Bank CDR Accounts & Balances API
  slug: qudos-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/openapi/qudos-bank-cds-banking-products-openapi.yml
- filename: qudos-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Qudos Bank CDR Transactions API
  slug: qudos-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/openapi/qudos-bank-cds-banking-products-openapi.yml
- filename: qudos-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Qudos Bank CDR Direct Debits & Scheduled Payments API
  slug: qudos-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/openapi/qudos-bank-cds-banking-products-openapi.yml
- filename: qudos-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Qudos Bank CDR Payees API
  slug: qudos-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/openapi/qudos-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qudosbank.com.au
  spf: true
hosts:
- cert_expires: Sep 30 04:30:12 2026 GMT
  host: www.qudosbank.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: public.cdr.qudosbank.com.au
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qudos Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qudos Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Qudos Bank
provider_slug: qudos-bank
slug: qudos-bank-domain-security
source_filename: qudos-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qudosbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 04:30:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.cdr.qudosbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\ndomains:\n- domain: qudosbank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/security/qudos-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Customer Owned
- Mutual Bank
- Product Reference Data
---
