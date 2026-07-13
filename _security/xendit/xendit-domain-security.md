---
api_specs:
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Payment Requests API
  slug: xendit-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Payment Tokens API
  slug: xendit-payment-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Invoices API
  slug: xendit-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Payouts API
  slug: xendit-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Balance API
  slug: xendit-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Transactions API
  slug: xendit-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Customers API
  slug: xendit-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Refunds API
  slug: xendit-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xendit.co
  spf: true
hosts:
- cert_expires: Oct  2 02:01:22 2026 GMT
  host: api.xendit.co
  hsts: false
  https: true
  note: Base API host. Returns HTTP 403 to unauthenticated root requests, as expected.
  tls_version: TLSv1.3
- cert_expires: Sep 25 14:27:55 2026 GMT
  host: www.xendit.co
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 07:09:56 2026 GMT
  host: docs.xendit.co
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xendit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xendit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Xendit
provider_slug: xendit
slug: xendit-domain-security
source_filename: xendit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.xendit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:01:22 2026 GMT\n  hsts: false\n  note: Base API host. Returns HTTP 403 to unauthenticated root requests, as expected.\n- host: www.xendit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:27:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n- host: docs.xendit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:09:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\ndomains:\n- domain: xendit.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/security/xendit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Fintech
- Payment Gateway
- Southeast Asia
- Indonesia
- Philippines
- Disbursements
- E-Wallet
- Virtual Accounts
- Cards
- Financial Infrastructure
---
