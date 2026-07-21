---
api_specs:
- filename: bank-of-melbourne-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Melbourne CDR Product Reference Data API
  slug: bank-of-melbourne-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-melbourne/refs/heads/main/openapi/bank-of-melbourne-cds-banking-products-openapi.yml
- filename: bank-of-melbourne-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Melbourne CDR Accounts & Balances API
  slug: bank-of-melbourne-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-melbourne/refs/heads/main/openapi/bank-of-melbourne-cds-banking-products-openapi.yml
- filename: bank-of-melbourne-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Melbourne CDR Transactions API
  slug: bank-of-melbourne-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-melbourne/refs/heads/main/openapi/bank-of-melbourne-cds-banking-products-openapi.yml
- filename: bank-of-melbourne-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Melbourne CDR Direct Debits & Scheduled Payments API
  slug: bank-of-melbourne-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-melbourne/refs/heads/main/openapi/bank-of-melbourne-cds-banking-products-openapi.yml
- filename: bank-of-melbourne-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Melbourne CDR Payees API
  slug: bank-of-melbourne-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-melbourne/refs/heads/main/openapi/bank-of-melbourne-cds-banking-products-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "entrust.net"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bankofmelbourne.com.au
  spf: true
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: www.bankofmelbourne.com.au
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: digital-api.bankofmelbourne.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bank Of Melbourne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bank of Melbourne, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bank of Melbourne
provider_slug: bank-of-melbourne
slug: bank-of-melbourne-domain-security
source_filename: bank-of-melbourne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bankofmelbourne.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: digital-api.bankofmelbourne.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bankofmelbourne.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-melbourne/refs/heads/main/security/bank-of-melbourne-domain-security.yml
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
- Westpac Group
---
