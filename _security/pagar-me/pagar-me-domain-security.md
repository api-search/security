---
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
- Credit Card
- Marketplace
- Split Payments
- Subscriptions
- Recurring Billing
- Anti-Fraud
- 3DS
- Checkout
- Payment Links
- Webhooks
- E-commerce
- Anticipation
---
