---
api_specs:
- filename: ludo-ai-audio-api-openapi.yml
  format: yaml
  label: Ludo.ai Audio API
  slug: ludo-ai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-audio-api-openapi.yml
- filename: ludo-ai-images-api-openapi.yml
  format: yaml
  label: Ludo.ai Images API
  slug: ludo-ai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-images-api-openapi.yml
- filename: ludo-ai-results-api-openapi.yml
  format: yaml
  label: Ludo.ai Results API
  slug: ludo-ai-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-results-api-openapi.yml
- filename: ludo-ai-video-api-openapi.yml
  format: yaml
  label: Ludo.ai Video API
  slug: ludo-ai-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-video-api-openapi.yml
- filename: ludo-ai-3d-models-api-openapi.yml
  format: yaml
  label: Ludo.ai 3D Models API
  slug: ludo-ai-3d-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-3d-models-api-openapi.yml
- filename: ludo-ai-account-api-openapi.yml
  format: yaml
  label: Ludo.ai Account API
  slug: ludo-ai-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-account-api-openapi.yml
- filename: ludo-ai-animation-api-openapi.yml
  format: yaml
  label: Ludo.ai Animation API
  slug: ludo-ai-animation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-animation-api-openapi.yml
- filename: ludo-ai-authentication-api-openapi.yml
  format: yaml
  label: Ludo.ai Authentication API
  slug: ludo-ai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-authentication-api-openapi.yml
- filename: ludo-ai-documentation-api-openapi.yml
  format: yaml
  label: Ludo.ai Documentation API
  slug: ludo-ai-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-documentation-api-openapi.yml
- filename: ludo-ai-files-api-openapi.yml
  format: yaml
  label: Ludo.ai Files API
  slug: ludo-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-files-api-openapi.yml
- filename: ludo-ai-generations-api-openapi.yml
  format: yaml
  label: Ludo.ai Generations API
  slug: ludo-ai-generations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-generations-api-openapi.yml
- filename: ludo-ai-jobs-api-openapi.yml
  format: yaml
  label: Ludo.ai Jobs API
  slug: ludo-ai-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-jobs-api-openapi.yml
- filename: ludo-ai-spritesheets-api-openapi.yml
  format: yaml
  label: Ludo.ai Spritesheets API
  slug: ludo-ai-spritesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-spritesheets-api-openapi.yml
- filename: ludo-ai-videos-api-openapi.yml
  format: yaml
  label: Ludo.ai Videos API
  slug: ludo-ai-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-videos-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ludo.ai
  spf: true
hosts:
- cert_expires: Nov 14 21:57:03 2026 GMT
  host: ludo.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 18:29:50 2026 GMT
  host: mcp.ludo.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 01:21:21 2026 GMT
  host: api.ludo.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Ludo Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ludo.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ludo.ai
provider_slug: ludo-ai
slug: ludo-ai-domain-security
source_filename: ludo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ludo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 21:57:03 2026 GMT\n  hsts: false\n- host: mcp.ludo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 18:29:50 2026 GMT\n  hsts: null\n- host: api.ludo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 01:21:21 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ludo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/security/ludo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Asset Generation
- Game Design
- Game Development
- Game Asset Generation
- AI Art
- Sprite Sheets
---
