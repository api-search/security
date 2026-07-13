---
api_specs:
- filename: hotelrunner-openapi.yml
  format: yaml
  label: HotelRunner Inventory API
  slug: hotelrunner-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelrunner/refs/heads/main/openapi/hotelrunner-openapi.yml
- filename: hotelrunner-openapi.yml
  format: yaml
  label: HotelRunner Reservations API
  slug: hotelrunner-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelrunner/refs/heads/main/openapi/hotelrunner-openapi.yml
- filename: hotelrunner-openapi.yml
  format: yaml
  label: HotelRunner Channels API
  slug: hotelrunner-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelrunner/refs/heads/main/openapi/hotelrunner-openapi.yml
- filename: hotelrunner-openapi.yml
  format: yaml
  label: HotelRunner Reference Data API
  slug: hotelrunner-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelrunner/refs/heads/main/openapi/hotelrunner-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hotelrunner.com
  spf: true
hosts:
- cert_expires: Dec 10 12:43:20 2026 GMT
  host: hotelrunner.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 12:43:20 2026 GMT
  host: developers.hotelrunner.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 10 12:43:20 2026 GMT
  host: app.hotelrunner.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hotelrunner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HotelRunner, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HotelRunner
provider_slug: hotelrunner
slug: hotelrunner-domain-security
source_filename: hotelrunner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hotelrunner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 12:43:20 2026 GMT\n  hsts: false\n- host: developers.hotelrunner.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 10 12:43:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.hotelrunner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 12:43:20 2026 GMT\n  hsts: false\ndomains:\n- domain: hotelrunner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotelrunner/refs/heads/main/security/hotelrunner-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hospitality
- Hotel
- Channel Manager
- Booking Engine
- PMS
- Travel
---
