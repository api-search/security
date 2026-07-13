---
api_specs:
- filename: api-spec.json
  format: json
  label: Mux Video API
  slug: video-api
  spec_type: OpenAPI
  url: https://www.mux.com/api-spec.json
- filename: api-spec.json
  format: json
  label: Mux Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://www.mux.com/api-spec.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mux.com
  spf: true
hosts:
- cert_expires: Aug  8 11:26:30 2026 GMT
  host: www.mux.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: api.mux.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mux, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mux
provider_slug: mux
slug: mux-domain-security
source_filename: mux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mux.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 11:26:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mux.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: mux.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mux/refs/heads/main/security/mux-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- Streaming
- Live Streaming
- Video Analytics
- QoE
- Video On Demand
- Transcoding
- Mux Player
---
