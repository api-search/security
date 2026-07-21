---
api_specs:
- filename: bankwest-cds-banking-products-openapi.yml
  format: yaml
  label: Bankwest CDR Product Reference Data API
  slug: bankwest-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-cds-banking-products-openapi.yml
- filename: bankwest-cds-banking-products-openapi.yml
  format: yaml
  label: Bankwest CDR Accounts & Balances API
  slug: bankwest-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-cds-banking-products-openapi.yml
- filename: bankwest-cds-banking-products-openapi.yml
  format: yaml
  label: Bankwest CDR Transactions API
  slug: bankwest-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-cds-banking-products-openapi.yml
- filename: bankwest-cds-banking-products-openapi.yml
  format: yaml
  label: Bankwest CDR Direct Debits & Scheduled Payments API
  slug: bankwest-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-cds-banking-products-openapi.yml
- filename: bankwest-cds-banking-products-openapi.yml
  format: yaml
  label: Bankwest CDR Payees API
  slug: bankwest-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bankwest.com.au
  spf: true
hosts:
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: www.bankwest.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: open-api.bankwest.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bankwest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bankwest, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bankwest
provider_slug: bankwest
slug: bankwest-domain-security
source_filename: bankwest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bankwest.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open-api.bankwest.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bankwest.com.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/security/bankwest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- Digital Bank
---
