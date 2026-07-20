---
api_specs:
- filename: openapi.yml
  format: yaml
  label: NOWPayments Payment API
  slug: nowpayments-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/now-payments/refs/heads/main/openapi/openapi.yml
- filename: S1a32n38
  format: yaml
  label: NOWPayments Mass Payouts API
  slug: nowpayments-mass-payouts-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/7907941/S1a32n38
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nowpayments.io
  spf: true
hosts:
- cert_expires: Aug 11 21:04:54 2026 GMT
  host: nowpayments.io
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 21:04:54 2026 GMT
  host: api.nowpayments.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.sandbox.nowpayments.io
  https: false
kind: domain-security
layout: security
method: probed
name: Now Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NOWPayments, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NOWPayments
provider_slug: now-payments
slug: now-payments-domain-security
source_filename: now-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nowpayments.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 21:04:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.nowpayments.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 21:04:54 2026 GMT\n  hsts: null\n- host: api.sandbox.nowpayments.io\n  https: false\ndomains:\n- domain: nowpayments.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/now-payments/refs/heads/main/security/now-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Crypto Payments
- Cryptocurrency
- Payment Gateway
- Invoicing
- Subscriptions
- Mass Payouts
- Bitcoin
- Ethereum
---
