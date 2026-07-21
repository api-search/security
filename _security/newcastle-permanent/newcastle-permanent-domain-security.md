---
api_specs:
- filename: newcastle-permanent-products-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Product Reference Data API
  slug: newcastle-permanent-cds-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-products-openapi.json
- filename: newcastle-permanent-customer-data-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Accounts & Balances API
  slug: newcastle-permanent-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-customer-data-openapi.json
- filename: newcastle-permanent-customer-data-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Transactions API
  slug: newcastle-permanent-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-customer-data-openapi.json
- filename: newcastle-permanent-customer-data-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Direct Debits & Scheduled Payments API
  slug: newcastle-permanent-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-customer-data-openapi.json
- filename: newcastle-permanent-customer-data-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Payees API
  slug: newcastle-permanent-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-customer-data-openapi.json
- filename: newcastle-permanent-customer-data-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Common Customer API
  slug: newcastle-permanent-cdr-common-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-customer-data-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: newcastlepermanent.com.au
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.newcastlepermanent.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: developer.newcastlepermanent.com.au
  hsts: true
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: openbank.newcastlepermanent.com.au
  hsts: true
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Newcastle Permanent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Newcastle Permanent Building Society, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Newcastle Permanent Building Society
provider_slug: newcastle-permanent
slug: newcastle-permanent-domain-security
source_filename: newcastle-permanent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.newcastlepermanent.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\n- host: developer.newcastlepermanent.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n- host: openbank.newcastlepermanent.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: true\ndomains:\n- domain: newcastlepermanent.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/security/newcastle-permanent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Building Society
- Mutual
- Australia
---
