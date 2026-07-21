---
api_specs:
- filename: ubank-cds-banking-products-openapi.yml
  format: yaml
  label: ubank CDR Product Reference Data API
  slug: ubank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-cds-banking-products-openapi.yml
- filename: ubank-cds-banking-products-openapi.yml
  format: yaml
  label: ubank CDR Banking Product Detail API
  slug: ubank-cdr-product-detail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-cds-banking-products-openapi.yml
- filename: ubank-cds-banking-products-openapi.yml
  format: yaml
  label: ubank CDR Accounts & Balances API
  slug: ubank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-cds-banking-products-openapi.yml
- filename: ubank-cds-banking-products-openapi.yml
  format: yaml
  label: ubank CDR Transactions API
  slug: ubank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-cds-banking-products-openapi.yml
- filename: ubank-cds-banking-products-openapi.yml
  format: yaml
  label: ubank CDR Direct Debits & Scheduled Payments API
  slug: ubank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-cds-banking-products-openapi.yml
- filename: ubank-cds-banking-products-openapi.yml
  format: yaml
  label: ubank CDR Payees API
  slug: ubank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ubank.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 86400.com.au
  spf: true
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: www.ubank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 16:00:04 2026 GMT
  host: public.cdr-api.86400.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ubank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ubank, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ubank
provider_slug: ubank
slug: ubank-domain-security
source_filename: ubank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ubank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: null\n- host: public.cdr-api.86400.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 16:00:04 2026 GMT\n  hsts: null\ndomains:\n- domain: ubank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: 86400.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/security/ubank-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial
- Banks
- Banking
- Open Banking
- CDR
- Consumer Data Right
- Product Reference Data
- Digital Bank
- Consumer Banking
- Australia
---
