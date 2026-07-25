---
api_specs:
- filename: vonage-video-archives-api-openapi.yml
  format: yaml
  label: Vonage Video API Archives API
  slug: vonage-video-archives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-archives-api-openapi.yml
- filename: vonage-video-broadcasts-api-openapi.yml
  format: yaml
  label: Vonage Video API Broadcasts API
  slug: vonage-video-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-broadcasts-api-openapi.yml
- filename: vonage-video-captions-api-openapi.yml
  format: yaml
  label: Vonage Video API Captions API
  slug: vonage-video-captions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-captions-api-openapi.yml
- filename: vonage-video-moderation-api-openapi.yml
  format: yaml
  label: Vonage Video API Moderation API
  slug: vonage-video-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-moderation-api-openapi.yml
- filename: vonage-video-render-api-openapi.yml
  format: yaml
  label: Vonage Video API Render API
  slug: vonage-video-render-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-render-api-openapi.yml
- filename: vonage-video-sessions-api-openapi.yml
  format: yaml
  label: Vonage Video API Sessions API
  slug: vonage-video-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-sessions-api-openapi.yml
- filename: vonage-video-signaling-api-openapi.yml
  format: yaml
  label: Vonage Video API Signaling API
  slug: vonage-video-signaling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-signaling-api-openapi.yml
- filename: vonage-video-sip-api-openapi.yml
  format: yaml
  label: Vonage Video API SIP API
  slug: vonage-video-sip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-sip-api-openapi.yml
- filename: vonage-video-streams-api-openapi.yml
  format: yaml
  label: Vonage Video API Streams API
  slug: vonage-video-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-streams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vonage.com
  spf: true
hosts:
- cert_expires: Oct  1 20:11:55 2026 GMT
  host: www.vonage.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: developer.vonage.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: video.api.vonage.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vonage Video Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vonage Video API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vonage Video API
provider_slug: vonage-video
slug: vonage-video-domain-security
source_filename: vonage-video-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vonage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:11:55 2026 GMT\n  hsts: null\n- host: developer.vonage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: video.api.vonage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: vonage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/security/vonage-video-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- WebRTC
- Live Streaming
- Real-Time Communications
- CPaaS
---
