---
api_specs:
- filename: sage-bank-accounts-api-openapi.yml
  format: yaml
  label: Sage Bank Accounts API
  slug: sage-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-bank-accounts-api-openapi.yml
- filename: sage-business-api-openapi.yml
  format: yaml
  label: Sage Business API
  slug: sage-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-business-api-openapi.yml
- filename: sage-contacts-api-openapi.yml
  format: yaml
  label: Sage Contacts API
  slug: sage-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-contacts-api-openapi.yml
- filename: sage-ledger-accounts-api-openapi.yml
  format: yaml
  label: Sage Ledger Accounts API
  slug: sage-ledger-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-ledger-accounts-api-openapi.yml
- filename: sage-payments-api-openapi.yml
  format: yaml
  label: Sage Payments API
  slug: sage-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-payments-api-openapi.yml
- filename: sage-products-api-openapi.yml
  format: yaml
  label: Sage Products API
  slug: sage-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-products-api-openapi.yml
- filename: sage-purchase-invoices-api-openapi.yml
  format: yaml
  label: Sage Purchase Invoices API
  slug: sage-purchase-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-purchase-invoices-api-openapi.yml
- filename: sage-sales-invoices-api-openapi.yml
  format: yaml
  label: Sage Sales Invoices API
  slug: sage-sales-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-sales-invoices-api-openapi.yml
- filename: sage-tax-rates-api-openapi.yml
  format: yaml
  label: Sage Tax Rates API
  slug: sage-tax-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-tax-rates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sage.com
  spf: true
hosts:
- cert_expires: Sep 29 04:04:19 2026 GMT
  host: developer.sage.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 23:59:59 2026 GMT
  host: www.sage.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.accounting.sage.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sage, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sage
provider_slug: sage
slug: sage-domain-security
source_filename: sage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.sage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:04:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.sage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.accounting.sage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/security/sage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Business Management
- Cloud Software
- ERP
- Payroll
- HR
---
