---
api_specs:
- filename: magichour-audio-projects-api-openapi.yml
  format: yaml
  label: Magic Hour Audio Projects API
  slug: magichour-audio-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magichour/refs/heads/main/openapi/magichour-audio-projects-api-openapi.yml
- filename: magichour-files-api-openapi.yml
  format: yaml
  label: Magic Hour Files API
  slug: magichour-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magichour/refs/heads/main/openapi/magichour-files-api-openapi.yml
- filename: magichour-image-projects-api-openapi.yml
  format: yaml
  label: Magic Hour Image Projects API
  slug: magichour-image-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magichour/refs/heads/main/openapi/magichour-image-projects-api-openapi.yml
- filename: magichour-video-projects-api-openapi.yml
  format: yaml
  label: Magic Hour Video Projects API
  slug: magichour-video-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magichour/refs/heads/main/openapi/magichour-video-projects-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: magichour.ai
  spf: true
hosts:
- cert_expires: Nov 26 03:01:52 2026 GMT
  host: magichour.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 15:26:03 2026 GMT
  host: docs.magichour.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 03:01:52 2026 GMT
  host: api.magichour.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Magichour Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magic Hour, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Magic Hour
provider_slug: magichour
slug: magichour-domain-security
source_filename: magichour-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magichour.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 03:01:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.magichour.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 15:26:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.magichour.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 03:01:52 2026 GMT\n  hsts: null\ndomains:\n- domain: magichour.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magichour/refs/heads/main/security/magichour-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Video
- Image-Generation
- Audio
- Generative AI
- Voice Cloning
- Text-To-Video
---
