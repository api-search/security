---
api_specs:
- filename: openapi.json
  format: json
  label: Mangopay REST API
  slug: mangopay-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mangopay/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mangopay.com
  spf: true
hosts:
- cert_expires: Aug 13 02:33:55 2026 GMT
  host: mangopay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 21:45:51 2026 GMT
  host: docs.mangopay.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: api.mangopay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mangopay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mangopay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mangopay
provider_slug: mangopay
slug: mangopay-domain-security
source_filename: mangopay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mangopay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 02:33:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mangopay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 21:45:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mangopay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mangopay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mangopay/refs/heads/main/security/mangopay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Marketplace Payments
- Digital Wallets
- KYC
- KYB
- Fund Transfers
- Currency Conversion
- Payment Cards
- Fintech
- European
---
