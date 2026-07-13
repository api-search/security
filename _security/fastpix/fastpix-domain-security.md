---
api_specs:
- filename: fastpix-openapi.yml
  format: yaml
  label: FastPix On-Demand API
  slug: fastpix-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-openapi.yml
- filename: fastpix-openapi.yml
  format: yaml
  label: FastPix Live Streaming API
  slug: fastpix-live-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-openapi.yml
- filename: fastpix-openapi.yml
  format: yaml
  label: FastPix Simulcast API
  slug: fastpix-simulcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-openapi.yml
- filename: fastpix-openapi.yml
  format: yaml
  label: FastPix Playback & Signing Keys API
  slug: fastpix-playback-signing-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-openapi.yml
- filename: fastpix-openapi.yml
  format: yaml
  label: FastPix In-Video AI API
  slug: fastpix-in-video-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-openapi.yml
- filename: fastpix-openapi.yml
  format: yaml
  label: FastPix Data & Views API
  slug: fastpix-data-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fastpix.io
  spf: true
hosts:
- cert_expires: Aug 25 14:35:34 2026 GMT
  host: www.fastpix.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 20:05:13 2026 GMT
  host: docs.fastpix.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 14:35:34 2026 GMT
  host: api.fastpix.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fastpix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FastPix, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FastPix
provider_slug: fastpix
slug: fastpix-domain-security
source_filename: fastpix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fastpix.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 14:35:34 2026 GMT\n  hsts: false\n- host: docs.fastpix.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:05:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.fastpix.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 14:35:34 2026 GMT\n  hsts: null\ndomains:\n- domain: fastpix.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/security/fastpix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- Streaming
- Live Streaming
- Video on Demand
- Encoding
- Playback
- Video Analytics
---
