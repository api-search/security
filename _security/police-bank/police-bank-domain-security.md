---
api_specs:
- filename: police-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Police Bank CDR Product Reference Data API
  slug: police-bank-cds-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/openapi/police-bank-cds-banking-products-openapi.yml
- filename: police-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Police Bank CDR Accounts & Balances API
  slug: police-bank-cds-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/openapi/police-bank-cds-banking-products-openapi.yml
- filename: police-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Police Bank CDR Transactions API
  slug: police-bank-cds-banking-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/openapi/police-bank-cds-banking-products-openapi.yml
- filename: police-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Police Bank CDR Direct Debits & Scheduled Payments API
  slug: police-bank-cds-banking-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/openapi/police-bank-cds-banking-products-openapi.yml
- filename: police-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Police Bank CDR Payees API
  slug: police-bank-cds-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/openapi/police-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: policebank.com.au
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.policebank.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: public.cdr.prd.policebank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Police Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Police Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Police Bank
provider_slug: police-bank
slug: police-bank-domain-security
source_filename: police-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.policebank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: public.cdr.prd.policebank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: policebank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/security/police-bank-domain-security.yml
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
