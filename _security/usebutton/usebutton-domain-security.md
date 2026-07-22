---
api_specs:
- filename: usebutton-brands-openapi.yml
  format: yaml
  label: Button Brands API
  slug: button-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usebutton/refs/heads/main/openapi/usebutton-brands-openapi.yml
- filename: usebutton-billing-openapi.yml
  format: yaml
  label: Button Billing API
  slug: button-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usebutton/refs/heads/main/openapi/usebutton-billing-openapi.yml
- filename: usebutton-links-openapi.yml
  format: yaml
  label: Button Links API
  slug: button-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usebutton/refs/heads/main/openapi/usebutton-links-openapi.yml
- filename: usebutton-shortlink-openapi.yml
  format: yaml
  label: Button Shortlink API
  slug: button-shortlink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usebutton/refs/heads/main/openapi/usebutton-shortlink-openapi.yml
- filename: usebutton-offers-openapi.yml
  format: yaml
  label: Button Offers API
  slug: button-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usebutton/refs/heads/main/openapi/usebutton-offers-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usebutton.com
  spf: true
hosts:
- cert_expires: Oct 14 16:39:33 2026 GMT
  host: usebutton.com
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
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: pubapi.usebutton.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Usebutton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Button, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Button
provider_slug: usebutton
slug: usebutton-domain-security
source_filename: usebutton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usebutton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:39:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.usebutton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pubapi.usebutton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usebutton.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usebutton/refs/heads/main/security/usebutton-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- Mobile Commerce
- Affiliate
- Attribution
- Deep Linking
- Offers
- Publishers
- Retail
---
