---
api_specs:
- filename: flipp-wishabi-flyerkit-openapi.yml
  format: yaml
  label: Flipp FlyerKit API
  slug: flipp-flyerkit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipp-wishabi/refs/heads/main/openapi/flipp-wishabi-flyerkit-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flipp.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.flipp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: api.flipp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flipp Wishabi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flipp (Wishabi), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flipp (Wishabi)
provider_slug: flipp-wishabi
slug: flipp-wishabi-domain-security
source_filename: flipp-wishabi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flipp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.flipp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: flipp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flipp-wishabi/refs/heads/main/security/flipp-wishabi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Retail Media
- Advertising
- Flyers
- Coupons
- E-commerce
- Shopping
- Marketing
- Digital Circulars
- Publications
- Merchandising
- Product Data
- Store Locator
---
