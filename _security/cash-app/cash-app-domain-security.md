---
api_specs:
- filename: cash-app-network-api-openapi.json
  format: json
  label: Cash App Pay Network API
  slug: cash-app-pay-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-network-api-openapi.json
- filename: cash-app-customer-request-api-openapi.json
  format: json
  label: Cash App Pay Customer Request API
  slug: cash-app-pay-customer-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-customer-request-api-openapi.json
- filename: cash-app-management-api-openapi.json
  format: json
  label: Cash App Pay Management API
  slug: cash-app-pay-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-management-api-openapi.json
- filename: cash-app-payments-openapi.json
  format: json
  label: Afterpay Payments API
  slug: afterpay-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-payments-openapi.json
- filename: cash-app-checkouts-openapi.json
  format: json
  label: Afterpay Checkouts API
  slug: afterpay-checkouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-checkouts-openapi.json
- filename: cash-app-orders-openapi.json
  format: json
  label: Afterpay Orders API
  slug: afterpay-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-orders-openapi.json
- filename: cash-app-configuration-openapi.json
  format: json
  label: Afterpay Configuration API
  slug: afterpay-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-configuration-openapi.json
- filename: cash-app-disputes-openapi.json
  format: json
  label: Afterpay Disputes API
  slug: afterpay-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-disputes-openapi.json
- filename: cash-app-grants-afterpay-openapi.json
  format: json
  label: Afterpay Grants API
  slug: afterpay-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-grants-afterpay-openapi.json
- filename: cash-app-grants-cash-app-pay-openapi.json
  format: json
  label: Add Cash App Pay to Your Site (Grants) API
  slug: cash-app-pay-site-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-grants-cash-app-pay-openapi.json
- filename: cash-app-service-status-openapi.json
  format: json
  label: Afterpay Service Status API
  slug: afterpay-service-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-service-status-openapi.json
- filename: cash-app-billing-agreements-deprecated-openapi.json
  format: json
  label: Afterpay Billing Agreements API (Deprecated)
  slug: afterpay-billing-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-billing-agreements-deprecated-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cash.app
  spf: true
hosts:
- cert_expires: Oct  8 23:31:29 2026 GMT
  host: cash.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 13:53:11 2026 GMT
  host: developers.cash.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 22:09:30 2026 GMT
  host: api.cash.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cash App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cash App, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cash App
provider_slug: cash-app
slug: cash-app-domain-security
source_filename: cash-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cash.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:31:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.cash.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 13:53:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cash.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 22:09:30 2026 GMT\n  hsts: null\ndomains:\n- domain: cash.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/security/cash-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Payments
- United States
- Fintech
- Neobank
- Buy Now Pay Later
- Payment Acceptance
- Digital Wallet
---
