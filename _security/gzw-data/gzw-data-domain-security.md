---
api_specs:
- filename: spec
  format: yaml
  label: GZW Data API
  slug: gzw-data-api
  spec_type: OpenAPI
  url: https://gzw-data.dev/api/v1/spec
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gzw-data.dev
  spf: false
hosts:
- cert_expires: Nov 24 16:07:18 2026 GMT
  host: gzw-data.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gzw Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GZW Data API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: GZW Data API
provider_slug: gzw-data
slug: gzw-data-domain-security
source_filename: gzw-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gzw-data.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 16:07:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gzw-data.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gzw-data/refs/heads/main/security/gzw-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- gaming
- video-games
- gray-zone-warfare
- game-data
- developer-tools
- open-data
- openapi
- weapons
- missions
- loot
- rest-api
- public-api
- no-auth
- read-only
- free-api
- community
---
