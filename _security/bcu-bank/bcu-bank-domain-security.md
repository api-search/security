---
api_specs:
- filename: bcu-bank-cds-banking-products-openapi.yml
  format: yaml
  label: BCU Bank CDR Product Reference Data API
  slug: bcu-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/openapi/bcu-bank-cds-banking-products-openapi.yml
- filename: bcu-bank-cds-banking-products-openapi.yml
  format: yaml
  label: BCU Bank CDR Accounts & Balances API
  slug: bcu-bank-cdr-accounts-and-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/openapi/bcu-bank-cds-banking-products-openapi.yml
- filename: bcu-bank-cds-banking-products-openapi.yml
  format: yaml
  label: BCU Bank CDR Transactions API
  slug: bcu-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/openapi/bcu-bank-cds-banking-products-openapi.yml
- filename: bcu-bank-cds-banking-products-openapi.yml
  format: yaml
  label: BCU Bank CDR Direct Debits & Scheduled Payments API
  slug: bcu-bank-cdr-direct-debits-and-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/openapi/bcu-bank-cds-banking-products-openapi.yml
- filename: bcu-bank-cds-banking-products-openapi.yml
  format: yaml
  label: BCU Bank CDR Payees API
  slug: bcu-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/openapi/bcu-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bcu.com.au
  spf: true
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: www.bcu.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 19:02:43 2026 GMT
  host: public.cdr-api.bcu.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bcu Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BCU Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BCU Bank
provider_slug: bcu-bank
slug: bcu-bank-domain-security
source_filename: bcu-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bcu.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.cdr-api.bcu.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 19:02:43 2026 GMT\n  hsts: null\ndomains:\n- domain: bcu.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/security/bcu-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Mutual Bank
- Australia
---
