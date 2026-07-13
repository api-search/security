---
api_specs:
- filename: rest-api-authentication
  format: yaml
  label: Product Fruits REST API
  slug: product-fruits-rest-api
  spec_type: OpenAPI
  url: https://help.productfruits.com/en/article/rest-api-authentication
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: productfruits.com
  spf: true
hosts:
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: productfruits.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: help.productfruits.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.productfruits.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Product Fruits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Product Fruits, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Product Fruits
provider_slug: product-fruits
slug: product-fruits-domain-security
source_filename: product-fruits-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: productfruits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.productfruits.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: false\n- host: api.productfruits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: productfruits.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/product-fruits/refs/heads/main/security/product-fruits-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Product Adoption
- User Onboarding
- In-App Guidance
- Checklists
- NPS Surveys
- Announcements
- User Segmentation
- SaaS
---
