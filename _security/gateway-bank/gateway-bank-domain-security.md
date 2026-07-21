---
api_specs:
- filename: gateway-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Gateway Bank CDR Product Reference Data API
  slug: gateway-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/openapi/gateway-bank-cds-banking-products-openapi.yml
- filename: gateway-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Gateway Bank CDR Accounts & Balances API
  slug: gateway-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/openapi/gateway-bank-cds-banking-products-openapi.yml
- filename: gateway-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Gateway Bank CDR Transactions API
  slug: gateway-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/openapi/gateway-bank-cds-banking-products-openapi.yml
- filename: gateway-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Gateway Bank CDR Direct Debits & Scheduled Payments API
  slug: gateway-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/openapi/gateway-bank-cds-banking-products-openapi.yml
- filename: gateway-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Gateway Bank CDR Payees API
  slug: gateway-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/openapi/gateway-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gatewaybank.com.au
  spf: true
hosts:
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: www.gatewaybank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 19:20:32 2026 GMT
  host: public.cdr-api.gatewaybank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gateway Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gateway Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gateway Bank
provider_slug: gateway-bank
slug: gateway-bank-domain-security
source_filename: gateway-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gatewaybank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: null\n- host: public.cdr-api.gatewaybank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 19:20:32 2026 GMT\n  hsts: null\ndomains:\n- domain: gatewaybank.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/security/gateway-bank-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Mutual Bank
- Customer Owned
- Australia
- Product Reference Data
---
