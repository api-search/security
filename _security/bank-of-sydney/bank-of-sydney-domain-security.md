---
api_specs:
- filename: bank-of-sydney-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Sydney CDR Product Reference Data API
  slug: bank-of-sydney-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/openapi/bank-of-sydney-cds-banking-products-openapi.yml
- filename: bank-of-sydney-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Sydney CDR Accounts & Balances API
  slug: bank-of-sydney-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/openapi/bank-of-sydney-cds-banking-products-openapi.yml
- filename: bank-of-sydney-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Sydney CDR Transactions API
  slug: bank-of-sydney-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/openapi/bank-of-sydney-cds-banking-products-openapi.yml
- filename: bank-of-sydney-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Sydney CDR Direct Debits & Scheduled Payments API
  slug: bank-of-sydney-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/openapi/bank-of-sydney-cds-banking-products-openapi.yml
- filename: bank-of-sydney-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Sydney CDR Payees API
  slug: bank-of-sydney-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/openapi/bank-of-sydney-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: banksyd.com.au
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.banksyd.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: openbank.api.banksyd.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bank Of Sydney Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bank of Sydney, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bank of Sydney
provider_slug: bank-of-sydney
slug: bank-of-sydney-domain-security
source_filename: bank-of-sydney-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.banksyd.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\n- host: openbank.api.banksyd.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: banksyd.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/security/bank-of-sydney-domain-security.yml
summary_line: TLSv1.3 · DMARC
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
