---
api_specs:
- filename: fawrypay-server-api-openapi.yml
  format: yaml
  label: FawryPay Server API
  slug: fawrypay-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fawry/refs/heads/main/openapi/fawrypay-server-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fawry.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fawrystaging.com
  spf: true
hosts:
- cert_expires: Aug 29 17:39:49 2026 GMT
  host: fawry.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 07:27:09 2026 GMT
  host: developer.fawrystaging.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  2 07:27:09 2026 GMT
  host: atfawry.fawrystaging.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fawry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fawry, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fawry
provider_slug: fawry
slug: fawry-domain-security
source_filename: fawry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fawry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 17:39:49 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: developer.fawrystaging.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 07:27:09 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: atfawry.fawrystaging.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 07:27:09 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: fawry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: fawrystaging.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fawry/refs/heads/main/security/fawry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- E-Payments
- Digital Finance
- Fintech
- Egypt
- Cards
- Wallets
- Bill Payments
- POS
- Micro-Finance
- Installments
- 3D Secure
- Refunds
- Webhooks
- Mobile SDK
- E-Commerce Plugins
- Magento
- Shopify
- WooCommerce
---
