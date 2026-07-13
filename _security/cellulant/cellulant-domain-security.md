---
api_specs:
- filename: cellulant-checkout-api-openapi.yml
  format: yaml
  label: Cellulant Tingg Checkout API
  slug: cellulant-tingg-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellulant/refs/heads/main/openapi/cellulant-checkout-api-openapi.yml
- filename: cellulant-payouts-api-openapi.yml
  format: yaml
  label: Cellulant Tingg Payouts API
  slug: cellulant-tingg-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellulant/refs/heads/main/openapi/cellulant-payouts-api-openapi.yml
- filename: cellulant-engage-api-openapi.yml
  format: yaml
  label: Cellulant Tingg Engage API
  slug: cellulant-tingg-engage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellulant/refs/heads/main/openapi/cellulant-engage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cellulant.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tingg.africa
  spf: true
hosts:
- cert_expires: Aug 25 09:19:15 2026 GMT
  host: www.cellulant.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 14:43:29 2026 GMT
  host: developer.tingg.africa
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 08:27:30 2026 GMT
  host: docs.tingg.africa
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cellulant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cellulant, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cellulant
provider_slug: cellulant
slug: cellulant-domain-security
source_filename: cellulant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cellulant.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 09:19:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.tingg.africa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:43:29 2026 GMT\n  hsts: false\n- host: docs.tingg.africa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 08:27:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cellulant.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tingg.africa\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cellulant/refs/heads/main/security/cellulant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Mobile Money
- Checkout
- Payouts
- Disbursement
- Africa
- Pan-African
- Fintech
- Bank Transfer
- Cards
- Airtime
- Bill Payment
- SMS
- OTP
- Tingg
---
