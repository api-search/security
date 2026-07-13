---
api_specs:
- filename: amadeus-media-hotel-content-openapi.yaml
  format: yaml
  label: Hotel Content API
  slug: hotel-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/openapi/amadeus-media-hotel-content-openapi.yaml
- filename: amadeus-media-hotel-list-openapi.yaml
  format: yaml
  label: Hotel List API
  slug: hotel-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/openapi/amadeus-media-hotel-list-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amadeus.com
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: developers.amadeus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: api.amadeus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  1 23:59:59 2026 GMT
  host: test.api.amadeus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amadeus Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amadeus Media, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Amadeus Media
provider_slug: amadeus-media
slug: amadeus-media-domain-security
source_filename: amadeus-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.amadeus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.amadeus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: null\n- host: test.api.amadeus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amadeus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/security/amadeus-media-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Content
- Hotels
- Images
- Media
- Travel
---
