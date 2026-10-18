---
api_specs:
- filename: pagar-me-contestations-api-openapi.yml
  format: yaml
  label: Pagar.me Contestations API
  slug: pagar-me-contestations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-contestations-api-openapi.yml
- filename: pagar-me-customers-api-openapi.yml
  format: yaml
  label: Pagar.me Customers API
  slug: pagar-me-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-customers-api-openapi.yml
- filename: pagar-me-disputas-api-openapi.yml
  format: yaml
  label: Pagar.me Disputas API
  slug: pagar-me-disputas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-disputas-api-openapi.yml
- filename: pagar-me-hooks-api-openapi.yml
  format: yaml
  label: Pagar.me Hooks API
  slug: pagar-me-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-hooks-api-openapi.yml
- filename: pagar-me-invoices-api-openapi.yml
  format: yaml
  label: Pagar.me Invoices API
  slug: pagar-me-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-invoices-api-openapi.yml
- filename: pagar-me-orders-api-openapi.yml
  format: yaml
  label: Pagar.me Orders API
  slug: pagar-me-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-orders-api-openapi.yml
- filename: pagar-me-paymentlinks-api-openapi.yml
  format: yaml
  label: Pagar.me Paymentlinks API
  slug: pagar-me-paymentlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-paymentlinks-api-openapi.yml
- filename: pagar-me-plans-api-openapi.yml
  format: yaml
  label: Pagar.me Plans API
  slug: pagar-me-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-plans-api-openapi.yml
- filename: pagar-me-recipients-api-openapi.yml
  format: yaml
  label: Pagar.me Recipients API
  slug: pagar-me-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-recipients-api-openapi.yml
- filename: pagar-me-settlement-obligations-api-openapi.yml
  format: yaml
  label: Pagar.me Settlement Obligations API
  slug: pagar-me-settlement-obligations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-settlement-obligations-api-openapi.yml
- filename: pagar-me-settlements-api-openapi.yml
  format: yaml
  label: Pagar.me Settlements API
  slug: pagar-me-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-settlements-api-openapi.yml
- filename: pagar-me-subscriptions-api-openapi.yml
  format: yaml
  label: Pagar.me Subscriptions API
  slug: pagar-me-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-subscriptions-api-openapi.yml
- filename: pagar-me-tokens-api-openapi.yml
  format: yaml
  label: Pagar.me Tokens API
  slug: pagar-me-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-tokens-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pagar.me
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: pagar.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  2 11:58:22 2026 GMT
  host: docs.pagar.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 06:48:03 2026 GMT
  host: api.pagar.me
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Pagar Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pagar.me, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pagar.me
provider_slug: pagar-me
slug: pagar-me-domain-security
source_filename: pagar-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pagar.me\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pagar.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:58:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pagar.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 06:48:03 2026 GMT\n  hsts: null\ndomains:\n- domain: pagar.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/security/pagar-me-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Payments
- Financial Services
- Fintech
- Brazil
- Latin America
- Stone Co
- Pix
- Boleto
- Credit Cards
- Marketplace
- Split Payments
- Subscription
- Recurring Billing
- Fraud Prevention
- 3D
- Checkout
- Payment Links
- Webhook
- E-Commerce
- Anticipation
---
