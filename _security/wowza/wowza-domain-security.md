---
api_specs:
- filename: wowza-video-openapi.yml
  format: yaml
  label: Wowza Video REST API
  slug: wowza-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wowza/refs/heads/main/openapi/wowza-video-openapi.yml
- filename: wowza-streaming-engine-openapi.yml
  format: yaml
  label: Wowza Streaming Engine REST API
  slug: wowza-streaming-engine-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wowza/refs/heads/main/openapi/wowza-streaming-engine-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wowza.com
  spf: true
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: www.wowza.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 01:39:55 2026 GMT
  host: developer.wowza.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: api.video.wowza.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wowza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wowza, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wowza
provider_slug: wowza
slug: wowza-domain-security
source_filename: wowza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wowza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\n- host: developer.wowza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 01:39:55 2026 GMT\n  hsts: false\n- host: api.video.wowza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: wowza.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wowza/refs/heads/main/security/wowza-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Video
- Streaming
- Live Streaming
- Video On Demand
- Transcoding
- Media Server
- RTMP
- RTSP
- SRT
- WebRTC
- HLS
- MPEG-DASH
- Real-Time Streaming
- Low Latency
- Video Player
- HTML5 Player
- DRM
- CDN
- Video Analytics
- QoE
- Webhooks
- Edge
- Surveillance
- OTT
---
