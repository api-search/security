---
api_specs:
- filename: razorpay-openapi.yml
  format: yaml
  label: Razorpay Core REST API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/razorpay/refs/heads/main/openapi/razorpay-openapi.yml
- filename: razorpay-webhooks-asyncapi.yml
  format: yaml
  label: Razorpay Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/razorpay/refs/heads/main/asyncapi/razorpay-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: razorpay.com
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: razorpay.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: api.razorpay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Razorpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Razorpay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Razorpay
provider_slug: razorpay
slug: razorpay-domain-security
source_filename: razorpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: razorpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\n- host: api.razorpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: razorpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/razorpay/refs/heads/main/security/razorpay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Gateway
- Fintech
- India
- UPI
- Subscriptions
- Payouts
- Checkout
---
