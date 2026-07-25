---
api_specs:
- filename: civitai-blobs-api-openapi.yml
  format: yaml
  label: Civitai Blobs API
  slug: civitai-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-blobs-api-openapi.yml
- filename: civitai-creators-api-openapi.yml
  format: yaml
  label: Civitai Creators API
  slug: civitai-creators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-creators-api-openapi.yml
- filename: civitai-enums-api-openapi.yml
  format: yaml
  label: Civitai Enums API
  slug: civitai-enums-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-enums-api-openapi.yml
- filename: civitai-images-api-openapi.yml
  format: yaml
  label: Civitai Images API
  slug: civitai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-images-api-openapi.yml
- filename: civitai-models-api-openapi.yml
  format: yaml
  label: Civitai Models API
  slug: civitai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-models-api-openapi.yml
- filename: civitai-modelversions-api-openapi.yml
  format: yaml
  label: Civitai ModelVersions API
  slug: civitai-modelversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-modelversions-api-openapi.yml
- filename: civitai-permissions-api-openapi.yml
  format: yaml
  label: Civitai Permissions API
  slug: civitai-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-permissions-api-openapi.yml
- filename: civitai-tags-api-openapi.yml
  format: yaml
  label: Civitai Tags API
  slug: civitai-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-tags-api-openapi.yml
- filename: civitai-users-api-openapi.yml
  format: yaml
  label: Civitai Users API
  slug: civitai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-users-api-openapi.yml
- filename: civitai-vault-api-openapi.yml
  format: yaml
  label: Civitai Vault API
  slug: civitai-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-vault-api-openapi.yml
- filename: civitai-workflows-api-openapi.yml
  format: yaml
  label: Civitai Workflows API
  slug: civitai-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: civitai.com
  spf: true
hosts:
- cert_expires: Oct  4 12:15:38 2026 GMT
  host: civitai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 08:35:56 2026 GMT
  host: developer.civitai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 21:36:04 2026 GMT
  host: orchestration.civitai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Civitai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Civitai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Civitai
provider_slug: civitai
slug: civitai-domain-security
source_filename: civitai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: civitai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 12:15:38 2026 GMT\n  hsts: false\n- host: developer.civitai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:35:56 2026 GMT\n  hsts: false\n- host: orchestration.civitai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:36:04 2026 GMT\n  hsts: null\ndomains:\n- domain: civitai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/security/civitai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Artificial Intelligence
- Image Generation
- Video Generation
- Stable Diffusion
- SDXL
- Flux
- LoRA
- Model Hosting
- Community
- Generative AI
---
