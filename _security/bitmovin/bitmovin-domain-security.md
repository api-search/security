---
api_specs:
- filename: llms.txt
  format: yaml
  label: Bitmovin Encoding API
  slug: encoding-api
  spec_type: OpenAPI
  url: https://developer.bitmovin.com/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bitmovin.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: bitmovin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 02:54:23 2026 GMT
  host: developer.bitmovin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 13:30:54 2026 GMT
  host: api.bitmovin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitmovin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitmovin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bitmovin
provider_slug: bitmovin
slug: bitmovin-domain-security
source_filename: bitmovin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitmovin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\n- host: developer.bitmovin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:54:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bitmovin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 13:30:54 2026 GMT\n  hsts: null\ndomains:\n- domain: bitmovin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/security/bitmovin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- Encoding
- Streaming
- Live Streaming
- VOD
- Adaptive Bitrate
- HLS
- DASH
- DRM
- Player
- Analytics
- Media
- Cloud
---
