---
api_specs:
- filename: red5-webrtc-streaming-asyncapi.yml
  format: yaml
  label: Red5 Pro WebRTC SDK
  slug: webrtc-sdk
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/asyncapi/red5-webrtc-streaming-asyncapi.yml
- filename: red5-admin-api-openapi.yml
  format: yaml
  label: Red5 Admin API
  slug: red5-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-admin-api-openapi.yml
- filename: red5-file-restreamer-api-openapi.yml
  format: yaml
  label: Red5 File Restreamer API
  slug: red5-file-restreamer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-file-restreamer-api-openapi.yml
- filename: red5-images-api-openapi.yml
  format: yaml
  label: Red5 Images API
  slug: red5-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-images-api-openapi.yml
- filename: red5-inputs-api-openapi.yml
  format: yaml
  label: Red5 Inputs API
  slug: red5-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-inputs-api-openapi.yml
- filename: red5-mixers-api-openapi.yml
  format: yaml
  label: Red5 Mixers API
  slug: red5-mixers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-mixers-api-openapi.yml
- filename: red5-provision-api-openapi.yml
  format: yaml
  label: Red5 Provision API
  slug: red5-provision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-provision-api-openapi.yml
- filename: red5-proxy-api-openapi.yml
  format: yaml
  label: Red5 Proxy API
  slug: red5-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-proxy-api-openapi.yml
- filename: red5-rtmp-restreamer-api-openapi.yml
  format: yaml
  label: Red5 RTMP Restreamer API
  slug: red5-rtmp-restreamer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-rtmp-restreamer-api-openapi.yml
- filename: red5-servlet-configuration-api-openapi.yml
  format: yaml
  label: Red5 Servlet Configuration API
  slug: red5-servlet-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-servlet-configuration-api-openapi.yml
- filename: red5-streams-api-openapi.yml
  format: yaml
  label: Red5 Streams API
  slug: red5-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-streams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: red5.net
  spf: true
hosts:
- cert_expires: Sep 17 23:45:17 2026 GMT
  host: www.red5.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Red5 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Red5, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Red5
provider_slug: red5
slug: red5-domain-security
source_filename: red5-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.red5.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:45:17 2026 GMT\n  hsts: false\ndomains:\n- domain: red5.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/security/red5-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Live Streaming
- Media
- Real-Time
- RTMP
- Streaming
- Video
- WebRTC
---
