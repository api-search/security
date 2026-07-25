---
api_specs:
- filename: xero-accounting-accounts-api-openapi.yml
  format: yaml
  label: Xero Accounting Accounts API
  slug: xero-accounting-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero-accounting/refs/heads/main/openapi/xero-accounting-accounts-api-openapi.yml
- filename: xero-accounting-banktransactions-api-openapi.yml
  format: yaml
  label: Xero Accounting BankTransactions API
  slug: xero-accounting-banktransactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero-accounting/refs/heads/main/openapi/xero-accounting-banktransactions-api-openapi.yml
- filename: xero-accounting-banktransfers-api-openapi.yml
  format: yaml
  label: Xero Accounting BankTransfers API
  slug: xero-accounting-banktransfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero-accounting/refs/heads/main/openapi/xero-accounting-banktransfers-api-openapi.yml
- filename: xero-accounting-batchpayments-api-openapi.yml
  format: yaml
  label: Xero Accounting BatchPayments API
  slug: xero-accounting-batchpayments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero-accounting/refs/heads/main/openapi/xero-accounting-batchpayments-api-openapi.yml
- filename: xero-accounting-contacts-api-openapi.yml
  format: yaml
  label: Xero Accounting Contacts API
  slug: xero-accounting-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero-accounting/refs/heads/main/openapi/xero-accounting-contacts-api-openapi.yml
- filename: xero-accounting-invoices-api-openapi.yml
  format: yaml
  label: Xero Accounting Invoices API
  slug: xero-accounting-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero-accounting/refs/heads/main/openapi/xero-accounting-invoices-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xero.com
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: www.xero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  2 22:00:00 2026 GMT
  host: developer.xero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: api.xero.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xero Accounting Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xero Accounting, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Xero Accounting
provider_slug: xero-accounting
slug: xero-accounting-domain-security
source_filename: xero-accounting-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\n- host: developer.xero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 22:00:00 2026 GMT\n  hsts: false\n- host: api.xero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: xero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xero-accounting/refs/heads/main/security/xero-accounting-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Accounting
- Small Business
- Invoicing
- Bookkeeping
- Financial Reporting
- SaaS
---
