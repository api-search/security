---
api_specs:
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Payments API
  slug: toss-payments-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Billing API
  slug: toss-payments-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Virtual Accounts API
  slug: toss-payments-virtual-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Cash Receipts API
  slug: toss-payments-cash-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Transactions API
  slug: toss-payments-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Settlements API
  slug: toss-payments-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Payouts API
  slug: toss-payments-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tosspayments.com
  spf: true
  spf_policy: ~all
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: tosspayments.com
  hsts: false
  http_status: 301
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  9 23:59:59 2027 GMT
  host: api.tosspayments.com
  hsts: false
  http_status: 401
  https: true
  note: A bare request to /v1/payments returns HTTP 401 (auth required), confirming the live authenticated REST surface.
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: docs.tosspayments.com
  hsts: false
  http_status: 308
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Toss Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toss Payments, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Toss Payments
provider_slug: toss-payments
slug: toss-payments-domain-security
source_filename: toss-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tosspayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\n  http_status: 301\n- host: api.tosspayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  9 23:59:59 2027 GMT\n  hsts: false\n  http_status: 401\n  note: A bare request to /v1/payments returns HTTP 401 (auth required), confirming the live authenticated REST surface.\n- host: docs.tosspayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\n  http_status: 308\ndomains:\n- domain: tosspayments.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: '~all'\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/security/toss-payments-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Payment Gateway
- South Korea
- Cards
- Easy Pay
- Virtual Account
- Billing
- Checkout
- Fintech
---
