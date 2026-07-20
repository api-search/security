---
api_specs:
- filename: button-brands-api-openapi.json
  format: json
  label: Button Brands API
  slug: button-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/openapi/button-brands-api-openapi.json
- filename: button-billing-api-openapi.json
  format: json
  label: Button Billing API
  slug: button-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/openapi/button-billing-api-openapi.json
- filename: button-links-api-openapi.json
  format: json
  label: Button Links API
  slug: button-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/openapi/button-links-api-openapi.json
- filename: button-shortlink-api-openapi.json
  format: json
  label: Button Shortlink API
  slug: button-shortlink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/openapi/button-shortlink-api-openapi.json
- filename: button-offers-api-openapi.json
  format: json
  label: Button Offers API
  slug: button-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/openapi/button-offers-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usebutton.com
  spf: true
hosts:
- cert_expires: Sep 30 16:07:11 2026 GMT
  host: www.usebutton.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 00:03:19 2026 GMT
  host: developer.usebutton.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: api.usebutton.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Button Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Button, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Button
provider_slug: button
slug: button-domain-security
source_filename: button-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usebutton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:07:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.usebutton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 00:03:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.usebutton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usebutton.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/security/button-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- Affiliate Marketing
- Mobile
- Attribution
- Deep Linking
- Retail Media
- Analytics
- Advertising
- Links
---
