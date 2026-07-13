---
api_specs:
- filename: bytark-openapi.yml
  format: yaml
  label: ByteArk Stream Video API
  slug: bytark-stream-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/openapi/bytark-openapi.yml
- filename: bytark-openapi.yml
  format: yaml
  label: ByteArk Live Streaming API
  slug: bytark-live-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/openapi/bytark-openapi.yml
- filename: bytark-openapi.yml
  format: yaml
  label: ByteArk Storage API
  slug: bytark-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/openapi/bytark-openapi.yml
- filename: bytark-openapi.yml
  format: yaml
  label: ByteArk CDN API
  slug: bytark-cdn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/openapi/bytark-openapi.yml
- filename: bytark-openapi.yml
  format: yaml
  label: ByteArk Player API
  slug: bytark-player-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/openapi/bytark-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: byteark.com
  spf: true
hosts:
- cert_expires: Oct  2 11:01:49 2026 GMT
  host: www.byteark.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 07:01:43 2026 GMT
  host: docs.byteark.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 11:09:02 2026 GMT
  host: stream.byteark.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bytark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ByteArk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ByteArk
provider_slug: bytark
slug: bytark-domain-security
source_filename: bytark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.byteark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:01:49 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.byteark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 07:01:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: stream.byteark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 11:09:02 2026 GMT\n  hsts: false\ndomains:\n- domain: byteark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/security/bytark-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- Streaming
- Video on Demand
- Live Streaming
- CDN
- Object Storage
- Transcoding
- DRM
- Media
---
