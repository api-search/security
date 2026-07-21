---
api_specs:
- filename: imb-bank-cds-banking-products-openapi.yml
  format: yaml
  label: IMB Bank CDR Product Reference Data API
  slug: imb-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-cds-banking-products-openapi.yml
- filename: imb-bank-cds-banking-products-openapi.yml
  format: yaml
  label: IMB Bank CDR Accounts & Balances API
  slug: imb-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-cds-banking-products-openapi.yml
- filename: imb-bank-cds-banking-products-openapi.yml
  format: yaml
  label: IMB Bank CDR Transactions API
  slug: imb-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-cds-banking-products-openapi.yml
- filename: imb-bank-cds-banking-products-openapi.yml
  format: yaml
  label: IMB Bank CDR Direct Debits & Scheduled Payments API
  slug: imb-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-cds-banking-products-openapi.yml
- filename: imb-bank-cds-banking-products-openapi.yml
  format: yaml
  label: IMB Bank CDR Payees API
  slug: imb-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: imb.com.au
  spf: true
hosts:
- cert_expires: Sep  9 13:30:52 2026 GMT
  host: www.imb.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: openbank.openbanking.imb.com.au
  hsts: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imb Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IMB Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: IMB Bank
provider_slug: imb-bank
slug: imb-bank-domain-security
source_filename: imb-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.imb.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 13:30:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: openbank.openbanking.imb.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: true\ndomains:\n- domain: imb.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/security/imb-bank-domain-security.yml
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
