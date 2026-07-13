---
api_specs:
- filename: 100ms-live-server-side-api-openapi.yml
  format: yaml
  label: 100ms Server-Side API
  slug: server-side-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/100ms-live/refs/heads/main/openapi/100ms-live-server-side-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 100ms.live
  spf: true
hosts:
- cert_expires: Aug 27 06:05:37 2026 GMT
  host: www.100ms.live
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: api.100ms.live
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 100Ms Live Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 100ms, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 100ms
provider_slug: 100ms-live
slug: 100ms-live-domain-security
source_filename: 100ms-live-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.100ms.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 06:05:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.100ms.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: 100ms.live\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/100ms-live/refs/heads/main/security/100ms-live-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Live Video
- Live Streaming
- Video Conferencing
- WebRTC
- HLS
- RTMP
- Recording
- Real-time Messaging
- Live Infrastructure
- India
---
