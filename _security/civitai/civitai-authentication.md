---
api_key_in: []
api_specs:
- filename: civitai-site-api-openapi.yml
  format: yaml
  label: Civitai Site API
  slug: civitai-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-site-api-openapi.yml
- filename: civitai-orchestration-api-openapi.yml
  format: yaml
  label: Civitai Orchestration API
  slug: civitai-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-orchestration-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Civitai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Civitai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Civitai
provider_slug: civitai
scheme_count: 1
schemes:
- bearerFormat: token
  description: Personal API token issued at https://civitai.com/user/account.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/civitai-orchestration-api-openapi.yml
  - openapi/civitai-site-api-openapi.yml
  type: http
slug: civitai-authentication
source_filename: civitai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/civitai-orchestration-api-openapi.yml, openapi/civitai-site-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  description: Personal API token issued at https://civitai.com/user/account.\n  sources:\n  - openapi/civitai-orchestration-api-openapi.yml\n  - openapi/civitai-site-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/authentication/civitai-authentication.yml
summary_line: http · 1 scheme
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
