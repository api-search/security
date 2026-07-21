---
api_specs:
- filename: racq-bank-cds-banking-products-openapi.yml
  format: yaml
  label: RACQ Bank CDR Product Reference Data API
  slug: racq-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-cds-banking-products-openapi.yml
- filename: racq-bank-cds-banking-products-openapi.yml
  format: yaml
  label: RACQ Bank CDR Accounts & Balances API
  slug: racq-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-cds-banking-products-openapi.yml
- filename: racq-bank-cds-banking-products-openapi.yml
  format: yaml
  label: RACQ Bank CDR Transactions API
  slug: racq-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-cds-banking-products-openapi.yml
- filename: racq-bank-cds-banking-products-openapi.yml
  format: yaml
  label: RACQ Bank CDR Direct Debits & Scheduled Payments API
  slug: racq-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-cds-banking-products-openapi.yml
- filename: racq-bank-cds-banking-products-openapi.yml
  format: yaml
  label: RACQ Bank CDR Payees API
  slug: racq-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: racq.com.au
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.racq.com.au
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: cdrbank.racq.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Racq Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RACQ Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RACQ Bank
provider_slug: racq-bank
slug: racq-bank-domain-security
source_filename: racq-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.racq.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: cdrbank.racq.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: racq.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/security/racq-bank-domain-security.yml
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
- Mutual
---
