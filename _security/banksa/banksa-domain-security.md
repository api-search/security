---
api_specs:
- filename: banksa-cds-banking-products-openapi.yml
  format: yaml
  label: BankSA CDR Product Reference Data API
  slug: banksa-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/openapi/banksa-cds-banking-products-openapi.yml
- filename: banksa-cds-banking-products-openapi.yml
  format: yaml
  label: BankSA CDR Accounts & Balances API
  slug: banksa-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/openapi/banksa-cds-banking-products-openapi.yml
- filename: banksa-cds-banking-products-openapi.yml
  format: yaml
  label: BankSA CDR Transactions API
  slug: banksa-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/openapi/banksa-cds-banking-products-openapi.yml
- filename: banksa-cds-banking-products-openapi.yml
  format: yaml
  label: BankSA CDR Direct Debits & Scheduled Payments API
  slug: banksa-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/openapi/banksa-cds-banking-products-openapi.yml
- filename: banksa-cds-banking-products-openapi.yml
  format: yaml
  label: BankSA CDR Payees API
  slug: banksa-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/openapi/banksa-cds-banking-products-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: banksa.com.au
  spf: true
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: www.banksa.com.au
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: digital-api.banksa.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Banksa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BankSA, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BankSA
provider_slug: banksa
slug: banksa-domain-security
source_filename: banksa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.banksa.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: digital-api.banksa.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: banksa.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/security/banksa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Product Reference Data
---
