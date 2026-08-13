---
api_specs:
- filename: thrivecart-api-openapi.yml
  format: yaml
  label: ThriveCart API
  slug: thrivecart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/openapi/thrivecart-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thrivecart.com
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: thrivecart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: developers.thrivecart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thrivecart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThriveCart, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ThriveCart
provider_slug: thrivecart
slug: thrivecart-domain-security
source_filename: thrivecart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thrivecart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.thrivecart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thrivecart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/security/thrivecart-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Checkout
- Shopping Cart
- Payments
- eCommerce
- Subscriptions
- Affiliate Marketing
- Learning Management
- Creator Economy
- Webhooks
---
