---
api_specs:
- filename: runway-video-generation-openapi.yml
  format: yaml
  label: Runway Video Generation API
  slug: video-generation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-video-generation-openapi.yml
- filename: runway-image-generation-openapi.yml
  format: yaml
  label: Runway Image Generation API
  slug: image-generation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-image-generation-openapi.yml
- filename: runway-characters-openapi.yml
  format: yaml
  label: Runway Characters API
  slug: characters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-characters-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: runwayml.com
  spf: true
hosts:
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: docs.dev.runwayml.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 03:40:46 2026 GMT
  host: runwayml.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: api.dev.runwayml.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Runway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Runway, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Runway
provider_slug: runway
slug: runway-domain-security
source_filename: runway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.dev.runwayml.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: runwayml.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 03:40:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.dev.runwayml.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: runwayml.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/security/runway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video Generation
- Image Generation
- Artificial Intelligence
- Machine Learning
- Generative AI
- Avatars
- Characters
- WebRTC
- Creative Tools
---
