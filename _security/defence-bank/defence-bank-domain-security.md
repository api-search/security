---
api_specs:
- filename: defence-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Defence Bank CDR Product Reference Data API
  slug: defence-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-cds-banking-products-openapi.yml
- filename: defence-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Defence Bank CDR Accounts & Balances API
  slug: defence-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-cds-banking-products-openapi.yml
- filename: defence-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Defence Bank CDR Transactions API
  slug: defence-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-cds-banking-products-openapi.yml
- filename: defence-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Defence Bank CDR Direct Debits & Scheduled Payments API
  slug: defence-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-cds-banking-products-openapi.yml
- filename: defence-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Defence Bank CDR Payees API
  slug: defence-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: defencebank.com.au
  spf: true
hosts:
- cert_expires: Sep 25 15:23:45 2026 GMT
  host: www.defencebank.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: product.defencebank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Defence Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defence Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Defence Bank
provider_slug: defence-bank
slug: defence-bank-domain-security
source_filename: defence-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.defencebank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 15:23:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: product.defencebank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: defencebank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/security/defence-bank-domain-security.yml
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
