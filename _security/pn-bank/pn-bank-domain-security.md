---
api_specs:
- filename: pn-bank-cds-banking-products-openapi.yml
  format: yaml
  label: P&N Bank CDR Product Reference Data API
  slug: pn-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pn-bank/refs/heads/main/openapi/pn-bank-cds-banking-products-openapi.yml
- filename: pn-bank-cds-banking-products-openapi.yml
  format: yaml
  label: P&N Bank CDR Accounts & Balances API
  slug: pn-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pn-bank/refs/heads/main/openapi/pn-bank-cds-banking-products-openapi.yml
- filename: pn-bank-cds-banking-products-openapi.yml
  format: yaml
  label: P&N Bank CDR Transactions API
  slug: pn-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pn-bank/refs/heads/main/openapi/pn-bank-cds-banking-products-openapi.yml
- filename: pn-bank-cds-banking-products-openapi.yml
  format: yaml
  label: P&N Bank CDR Direct Debits & Scheduled Payments API
  slug: pn-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pn-bank/refs/heads/main/openapi/pn-bank-cds-banking-products-openapi.yml
- filename: pn-bank-cds-banking-products-openapi.yml
  format: yaml
  label: P&N Bank CDR Payees API
  slug: pn-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pn-bank/refs/heads/main/openapi/pn-bank-cds-banking-products-openapi.yml
- filename: pn-bank-cds-banking-products-openapi.yml
  format: yaml
  label: P&N Bank CDR Common Discovery API
  slug: pn-bank-cdr-common-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pn-bank/refs/heads/main/openapi/pn-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:domainalerts@pnbank.com.au"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pnbank.com.au
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: www.pnbank.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 20:30:36 2026 GMT
  host: public.cdr-api.pnbank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pn Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for P&N Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: P&N Bank
provider_slug: pn-bank
slug: pn-bank-domain-security
source_filename: pn-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pnbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.cdr-api.pnbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 20:30:36 2026 GMT\n  hsts: null\ndomains:\n- domain: pnbank.com.au\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:domainalerts@pnbank.com.au\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pn-bank/refs/heads/main/security/pn-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Customer Owned
- Product Reference Data
---
