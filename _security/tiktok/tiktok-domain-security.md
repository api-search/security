---
api_specs:
- filename: tiktok-business-openapi.yml
  format: yaml
  label: TikTok API for Business
  slug: tiktok-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-business-openapi.yml
- filename: tiktok-shop-openapi.yml
  format: yaml
  label: TikTok Shop API
  slug: tiktok-shop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-shop-openapi.yml
- filename: tiktok-data-portability-openapi.yml
  format: yaml
  label: TikTok Data Portability API
  slug: tiktok-data-portability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-data-portability-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tiktok.com
  spf: true
hosts:
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: www.tiktok.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: developers.tiktok.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: business-api.tiktok.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tiktok Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TikTok, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TikTok
provider_slug: tiktok
slug: tiktok-domain-security
source_filename: tiktok-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tiktok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.tiktok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\n- host: business-api.tiktok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tiktok.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/security/tiktok-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Commerce
- Content
- E-Commerce
- Social Media
- Video
---
