---
api_specs:
- filename: window-sticker-vin-api-openapi.yml
  format: yaml
  label: Window Sticker VIN API
  slug: window-sticker-vin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/window-sticker-vin-api/refs/heads/main/openapi/window-sticker-vin-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: windowsticker.org
  spf: true
hosts:
- cert_expires: Nov 24 17:49:16 2026 GMT
  host: windowsticker.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Window Sticker Vin Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Window Sticker VIN API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Window Sticker VIN API
provider_slug: window-sticker-vin-api
slug: window-sticker-vin-api-domain-security
source_filename: window-sticker-vin-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: windowsticker.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 17:49:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: windowsticker.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/window-sticker-vin-api/refs/heads/main/security/window-sticker-vin-api-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Automotive
- Vehicle Data
- VIN Decoding
- Monroney
- Window sticker
- Government open data
- Auto Retail
- Dealer tooling
---
