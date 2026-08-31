---
api_specs:
- filename: decart-realtime-api-openapi.yml
  format: yaml
  label: Decart Realtime API
  slug: decart-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decart/refs/heads/main/openapi/decart-realtime-api-openapi.yml
- filename: decart-client-api-openapi.yml
  format: yaml
  label: Decart Client API
  slug: decart-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decart/refs/heads/main/openapi/decart-client-api-openapi.yml
- filename: decart-files-api-openapi.yml
  format: yaml
  label: Decart Files API
  slug: decart-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decart/refs/heads/main/openapi/decart-files-api-openapi.yml
- filename: decart-generate-api-openapi.yml
  format: yaml
  label: Decart Generate API
  slug: decart-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decart/refs/heads/main/openapi/decart-generate-api-openapi.yml
- filename: decart-jobs-api-openapi.yml
  format: yaml
  label: Decart Jobs API
  slug: decart-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decart/refs/heads/main/openapi/decart-jobs-api-openapi.yml
- filename: decart-models-api-openapi.yml
  format: yaml
  label: Decart Models API
  slug: decart-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decart/refs/heads/main/openapi/decart-models-api-openapi.yml
- filename: decart-realtime-api-openapi.yml
  format: yaml
  label: Decart Realtime API
  slug: decart-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decart/refs/heads/main/openapi/decart-realtime-api-openapi.yml
- filename: decart-verify-api-openapi.yml
  format: yaml
  label: Decart Verify API
  slug: decart-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decart/refs/heads/main/openapi/decart-verify-api-openapi.yml
- filename: decart-watch-stream-api-openapi.yml
  format: yaml
  label: Decart Watch Stream API
  slug: decart-watch-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decart/refs/heads/main/openapi/decart-watch-stream-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: decart.ai
  spf: true
hosts:
- cert_expires: Oct 15 18:38:27 2026 GMT
  host: decart.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 03:55:18 2026 GMT
  host: docs.platform.decart.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: api.decart.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Decart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Decart, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Decart
provider_slug: decart
slug: decart-domain-security
source_filename: decart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: decart.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 18:38:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.platform.decart.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 03:55:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.decart.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: decart.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decart/refs/heads/main/security/decart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Machine-Learning
- Video
- Video Generation
- Video Editing
- Image Editing
- Real-Time
- Generative AI
- World Models
- Streaming
- WebRTC
- Media
- Developer Tools
- Company
---
