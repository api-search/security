---
api_specs:
- filename: bank-australia-cds-banking-openapi.json
  format: json
  label: Bank Australia CDR Product Reference Data API
  slug: bank-australia-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-cds-banking-openapi.json
- filename: bank-australia-cds-banking-openapi.json
  format: json
  label: Bank Australia CDR Accounts & Balances API
  slug: bank-australia-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-cds-banking-openapi.json
- filename: bank-australia-cds-banking-openapi.json
  format: json
  label: Bank Australia CDR Transactions API
  slug: bank-australia-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-cds-banking-openapi.json
- filename: bank-australia-cds-banking-openapi.json
  format: json
  label: Bank Australia CDR Direct Debits & Scheduled Payments API
  slug: bank-australia-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-cds-banking-openapi.json
- filename: bank-australia-cds-banking-openapi.json
  format: json
  label: Bank Australia CDR Payees API
  slug: bank-australia-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/openapi/bank-australia-cds-banking-openapi.json
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
