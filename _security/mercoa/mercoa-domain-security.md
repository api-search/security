---
api_specs:
- filename: mercoa-entities-api-openapi.yml
  format: yaml
  label: Mercoa Entities API
  slug: mercoa-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-entities-api-openapi.yml
- filename: mercoa-entity-groups-api-openapi.yml
  format: yaml
  label: Mercoa Entity Groups API
  slug: mercoa-entity-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-entity-groups-api-openapi.yml
- filename: mercoa-invoice-templates-api-openapi.yml
  format: yaml
  label: Mercoa Invoice Templates API
  slug: mercoa-invoice-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-invoice-templates-api-openapi.yml
- filename: mercoa-invoices-api-openapi.yml
  format: yaml
  label: Mercoa Invoices API
  slug: mercoa-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-invoices-api-openapi.yml
- filename: mercoa-ocr-api-openapi.yml
  format: yaml
  label: Mercoa OCR API
  slug: mercoa-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-ocr-api-openapi.yml
- filename: mercoa-organization-api-openapi.yml
  format: yaml
  label: Mercoa Organization API
  slug: mercoa-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-organization-api-openapi.yml
- filename: mercoa-payment-gateway-api-openapi.yml
  format: yaml
  label: Mercoa Payment Gateway API
  slug: mercoa-payment-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-payment-gateway-api-openapi.yml
- filename: mercoa-payment-methods-api-openapi.yml
  format: yaml
  label: Mercoa Payment Methods API
  slug: mercoa-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-payment-methods-api-openapi.yml
- filename: mercoa-transactions-api-openapi.yml
  format: yaml
  label: Mercoa Transactions API
  slug: mercoa-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mercoa.com
  spf: true
hosts:
- cert_expires: Oct  7 00:42:23 2026 GMT
  host: mercoa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 05:29:52 2026 GMT
  host: docs.mercoa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 00:42:23 2026 GMT
  host: api.mercoa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mercoa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mercoa, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mercoa
provider_slug: mercoa
slug: mercoa-domain-security
source_filename: mercoa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mercoa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 00:42:23 2026 GMT\n  hsts: false\n- host: docs.mercoa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 05:29:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mercoa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 00:42:23 2026 GMT\n  hsts: null\ndomains:\n- domain: mercoa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/security/mercoa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mercoa
- Embedded Finance
- Accounts Payable
- Accounts Receivable
- BillPay
- Invoicing
- Payments
- Vertical SaaS
- Vendors
- Approvals
- Disbursements
- Virtual Cards
---
