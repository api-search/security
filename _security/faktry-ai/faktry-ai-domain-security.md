---
api_specs:
- filename: faktry-ai-audio-api-openapi.yml
  format: yaml
  label: faktry Audio API
  slug: faktry-ai-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faktry-ai/openapi/faktry-ai-audio-api-openapi.yml
- filename: faktry-ai-image-api-openapi.yml
  format: yaml
  label: faktry Image API
  slug: faktry-ai-image-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faktry-ai/openapi/faktry-ai-image-api-openapi.yml
- filename: faktry-ai-pdf-api-openapi.yml
  format: yaml
  label: faktry PDF API
  slug: faktry-ai-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faktry-ai/openapi/faktry-ai-pdf-api-openapi.yml
- filename: faktry-ai-video-api-openapi.yml
  format: yaml
  label: faktry Video API
  slug: faktry-ai-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faktry-ai/openapi/faktry-ai-video-api-openapi.yml
- filename: faktry-ai-3-d-api-openapi.yml
  format: yaml
  label: faktry 3 D API
  slug: faktry-ai-3-d-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faktry-ai/openapi/faktry-ai-3-d-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: faktry.ai
  spf: true
hosts:
- cert_expires: Dec 12 23:57:03 2026 GMT
  host: faktry.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: faktry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for faktry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: faktry
provider_slug: faktry-ai
slug: faktry-ai-domain-security
source_filename: faktry-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: faktry.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:57:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: faktry.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/faktry-ai/security/faktry-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Media
- Platform
- Software-as-a-Service
- Image
- Video
- Audio
- 3D
---
