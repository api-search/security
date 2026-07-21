---
api_specs:
- filename: judo-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Judo Bank CDR Product Reference Data API
  slug: judo-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/openapi/judo-bank-cds-banking-products-openapi.yml
- filename: judo-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Judo Bank CDR Accounts & Balances API
  slug: judo-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/openapi/judo-bank-cds-banking-products-openapi.yml
- filename: judo-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Judo Bank CDR Transactions API
  slug: judo-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/openapi/judo-bank-cds-banking-products-openapi.yml
- filename: judo-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Judo Bank CDR Direct Debits & Scheduled Payments API
  slug: judo-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/openapi/judo-bank-cds-banking-products-openapi.yml
- filename: judo-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Judo Bank CDR Payees API
  slug: judo-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/openapi/judo-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: judo.bank
  spf: true
hosts:
- cert_expires: Oct 16 02:24:30 2026 GMT
  host: www.judo.bank
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: public.open.judo.bank
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Judo Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Judo Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Judo Bank
provider_slug: judo-bank
slug: judo-bank-domain-security
source_filename: judo-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.judo.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 02:24:30 2026 GMT\n  hsts: null\n- host: public.open.judo.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: judo.bank\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/security/judo-bank-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- SME Lending
- Product Reference Data
---
