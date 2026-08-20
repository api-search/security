---
api_specs:
- filename: modulr-api.json
  format: json
  label: Modulr Accounts API
  slug: modulr-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
- filename: modulr-api.json
  format: json
  label: Modulr Payments API
  slug: modulr-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
- filename: modulr-api.json
  format: json
  label: Modulr Cards API
  slug: modulr-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
- filename: modulr-api.json
  format: json
  label: Modulr Direct Debits API
  slug: modulr-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
- filename: modulr-api.json
  format: json
  label: Modulr Customers API
  slug: modulr-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
- filename: modulr-api.json
  format: json
  label: Modulr Payee Verification API
  slug: modulr-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
- filename: modulr-api.json
  format: json
  label: Modulr Payment Initiation API
  slug: modulr-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
- filename: modulr-api.json
  format: json
  label: Modulr Variable Recurring Payments API
  slug: modulr-variable-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
- filename: modulr-api.json
  format: json
  label: Modulr Notifications API
  slug: modulr-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/openapi/modulr-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: modulrfinance.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 16 19:47:40 2026 GMT
  host: www.modulrfinance.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: modulr.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.modulrfinance.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modulr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modulr, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Modulr
provider_slug: modulr
slug: modulr-domain-security
source_filename: modulr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.modulrfinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 19:47:40 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\n- host: modulr.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.modulrfinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: modulrfinance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modulr/refs/heads/main/security/modulr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- United Kingdom
- Banking as a Service
- Embedded Finance
- Payment Processing
- Account-to-Account
- Open Banking
- Faster Payments
- Card Issuing
- Direct Debit
- Confirmation of Payee
- Variable Recurring Payments
---
