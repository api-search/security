---
api_specs:
- filename: zoho-invoice-contacts-api-openapi.yml
  format: yaml
  label: Zoho Invoice Contacts API
  slug: zoho-invoice-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-invoice/refs/heads/main/openapi/zoho-invoice-contacts-api-openapi.yml
- filename: zoho-invoice-credit-notes-api-openapi.yml
  format: yaml
  label: Zoho Invoice Credit Notes API
  slug: zoho-invoice-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-invoice/refs/heads/main/openapi/zoho-invoice-credit-notes-api-openapi.yml
- filename: zoho-invoice-estimates-api-openapi.yml
  format: yaml
  label: Zoho Invoice Estimates API
  slug: zoho-invoice-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-invoice/refs/heads/main/openapi/zoho-invoice-estimates-api-openapi.yml
- filename: zoho-invoice-invoices-api-openapi.yml
  format: yaml
  label: Zoho Invoice Invoices API
  slug: zoho-invoice-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-invoice/refs/heads/main/openapi/zoho-invoice-invoices-api-openapi.yml
- filename: zoho-invoice-organizations-api-openapi.yml
  format: yaml
  label: Zoho Invoice Organizations API
  slug: zoho-invoice-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-invoice/refs/heads/main/openapi/zoho-invoice-organizations-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoho.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: zohoapis.com
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.zoho.com
  hsts: true
  hsts_max_age: 64072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: www.zohoapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zoho Invoice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zoho Invoice, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zoho Invoice
provider_slug: zoho-invoice
slug: zoho-invoice-domain-security
source_filename: zoho-invoice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zoho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 64072000\n- host: www.zohoapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zoho.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zohoapis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-invoice/refs/heads/main/security/zoho-invoice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Invoicing
- Accounting
- Small Business
- Billing
- Expense Tracking
- SaaS
---
