---
api_specs:
- filename: teachers-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Teachers Mutual Bank CDR Product Reference Data API
  slug: teachers-mutual-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/openapi/teachers-mutual-bank-cds-banking-products-openapi.yml
- filename: teachers-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Teachers Mutual Bank CDR Accounts & Balances API
  slug: teachers-mutual-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/openapi/teachers-mutual-bank-cds-banking-products-openapi.yml
- filename: teachers-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Teachers Mutual Bank CDR Transactions API
  slug: teachers-mutual-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/openapi/teachers-mutual-bank-cds-banking-products-openapi.yml
- filename: teachers-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Teachers Mutual Bank CDR Direct Debits & Scheduled Payments API
  slug: teachers-mutual-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/openapi/teachers-mutual-bank-cds-banking-products-openapi.yml
- filename: teachers-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Teachers Mutual Bank CDR Payees API
  slug: teachers-mutual-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/openapi/teachers-mutual-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tmbank.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tmbl.com.au
  spf: true
hosts:
- cert_expires: Aug 26 06:18:34 2026 GMT
  host: www.tmbank.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 00:11:59 2026 GMT
  host: ob.tmbl.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teachers Mutual Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teachers Mutual Bank, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Teachers Mutual Bank
provider_slug: teachers-mutual-bank
slug: teachers-mutual-bank-domain-security
source_filename: teachers-mutual-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tmbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 06:18:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ob.tmbl.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 00:11:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tmbank.com.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tmbl.com.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/security/teachers-mutual-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
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
