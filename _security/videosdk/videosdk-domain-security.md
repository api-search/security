---
api_specs:
- filename: videosdk-realtime-communication-api-openapi.yml
  format: yaml
  label: VideoSDK Real-Time Communication API
  slug: realtime-communication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videosdk/refs/heads/main/openapi/videosdk-realtime-communication-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: videosdk.live
  spf: true
hosts:
- cert_expires: Sep 28 17:49:41 2026 GMT
  host: www.videosdk.live
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 17:48:18 2026 GMT
  host: docs.videosdk.live
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 14 17:24:03 2026 GMT
  host: api.videosdk.live
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Videosdk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VideoSDK, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VideoSDK
provider_slug: videosdk
slug: videosdk-domain-security
source_filename: videosdk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.videosdk.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 17:49:41 2026 GMT\n  hsts: false\n- host: docs.videosdk.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 17:48:18 2026 GMT\n  hsts: false\n- host: api.videosdk.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 14 17:24:03 2026 GMT\n  hsts: null\ndomains:\n- domain: videosdk.live\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/videosdk/refs/heads/main/security/videosdk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Video
- Audio
- WebRTC
- Real-Time Communication
- Live Streaming
- HLS
- RTMP
- AI Agents
- Video Conferencing
- WebSocket
---
