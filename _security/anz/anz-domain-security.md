---
api_specs:
- filename: anz-cds-banking-products-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) CDR Product Reference Data API
  slug: anz-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-cds-banking-products-openapi.yml
- filename: anz-cds-banking-products-openapi.yml
  format: yaml
  label: ANZ Plus CDR Product Reference Data API
  slug: anz-plus-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-cds-banking-products-openapi.yml
- filename: anz-cds-banking-products-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) CDR Accounts & Balances API
  slug: anz-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-cds-banking-products-openapi.yml
- filename: anz-cds-banking-products-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) CDR Transactions API
  slug: anz-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-cds-banking-products-openapi.yml
- filename: anz-cds-banking-products-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) CDR Direct Debits & Scheduled Payments API
  slug: anz-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-cds-banking-products-openapi.yml
- filename: anz-cds-banking-products-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) CDR Payees API
  slug: anz-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-cds-banking-products-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anz.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: api.anz
  spf: false
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.anz.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: api.anz
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 26 09:56:47 2026 GMT
  host: cdr.apix.anz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Australia and New Zealand Banking Group (ANZ), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Australia and New Zealand Banking Group (ANZ)
provider_slug: anz
slug: anz-domain-security
source_filename: anz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anz.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\n- host: api.anz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\n- host: cdr.apix.anz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 26 09:56:47 2026 GMT\n  hsts: null\ndomains:\n- domain: anz.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: api.anz\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/security/anz-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
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
