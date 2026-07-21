---
api_specs:
- filename: st-george-bank-cds-banking-products-openapi.yml
  format: yaml
  label: St.George Bank CDR Product Reference Data API
  slug: st-george-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/openapi/st-george-bank-cds-banking-products-openapi.yml
- filename: st-george-bank-cds-banking-products-openapi.yml
  format: yaml
  label: St.George Bank CDR Accounts & Balances API
  slug: st-george-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/openapi/st-george-bank-cds-banking-products-openapi.yml
- filename: st-george-bank-cds-banking-products-openapi.yml
  format: yaml
  label: St.George Bank CDR Transactions API
  slug: st-george-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/openapi/st-george-bank-cds-banking-products-openapi.yml
- filename: st-george-bank-cds-banking-products-openapi.yml
  format: yaml
  label: St.George Bank CDR Direct Debits & Scheduled Payments API
  slug: st-george-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/openapi/st-george-bank-cds-banking-products-openapi.yml
- filename: st-george-bank-cds-banking-products-openapi.yml
  format: yaml
  label: St.George Bank CDR Payees API
  slug: st-george-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/openapi/st-george-bank-cds-banking-products-openapi.yml
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
  domain: stgeorge.com.au
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: www.stgeorge.com.au
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: digital-api.stgeorge.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: St George Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for St.George Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: St.George Bank
provider_slug: st-george-bank
slug: st-george-bank-domain-security
source_filename: st-george-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stgeorge.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: digital-api.stgeorge.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: stgeorge.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/security/st-george-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- Westpac Group
---
