---
api_key_in: []
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
