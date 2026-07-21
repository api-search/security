---
api_specs:
- filename: national-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: National Australia Bank (NAB) CDR Product Reference Data API
  slug: national-australia-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-cds-banking-products-openapi.yml
- filename: national-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: National Australia Bank (NAB) CDR Accounts & Balances API
  slug: national-australia-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-cds-banking-products-openapi.yml
- filename: national-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: National Australia Bank (NAB) CDR Transactions API
  slug: national-australia-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-cds-banking-products-openapi.yml
- filename: national-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: National Australia Bank (NAB) CDR Direct Debits & Scheduled Payments API
  slug: national-australia-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-cds-banking-products-openapi.yml
- filename: national-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: National Australia Bank (NAB) CDR Payees API
  slug: national-australia-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nab.com.au
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.nab.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: developer.nab.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: openbank.api.nab.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Australia Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Australia Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: National Australia Bank
provider_slug: national-australia-bank
slug: national-australia-bank-domain-security
source_filename: national-australia-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nab.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.nab.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\n- host: openbank.api.nab.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nab.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/security/national-australia-bank-domain-security.yml
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
