---
api_specs:
- filename: appcharge-openapi.yml
  format: yaml
  label: Appcharge Publisher API
  slug: appcharge-publisher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: appcharge.com
  spf: true
hosts:
- cert_expires: Sep 13 14:58:44 2026 GMT
  host: appcharge.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: api.appcharge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: api-sandbox.appcharge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appcharge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appcharge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Appcharge
provider_slug: appcharge
slug: appcharge-domain-security
source_filename: appcharge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appcharge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 14:58:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.appcharge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: null\n- host: api-sandbox.appcharge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: appcharge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/security/appcharge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Monetization
- Merchant of Record
- Mobile Games
- Gaming
- Checkout
- In-Game Purchases
- Web Store
- eCommerce
---
