---
api_key_in: []
api_specs:
- filename: recraft-ai-images-api-openapi.yml
  format: yaml
  label: Recraft Images API
  slug: recraft-ai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recraft-ai/refs/heads/main/openapi/recraft-ai-images-api-openapi.yml
- filename: recraft-ai-prompts-api-openapi.yml
  format: yaml
  label: Recraft Prompts API
  slug: recraft-ai-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recraft-ai/refs/heads/main/openapi/recraft-ai-prompts-api-openapi.yml
- filename: recraft-ai-styles-api-openapi.yml
  format: yaml
  label: Recraft Styles API
  slug: recraft-ai-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recraft-ai/refs/heads/main/openapi/recraft-ai-styles-api-openapi.yml
- filename: recraft-ai-users-api-openapi.yml
  format: yaml
  label: Recraft Users API
  slug: recraft-ai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recraft-ai/refs/heads/main/openapi/recraft-ai-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Recraft Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Recraft secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Recraft
provider_slug: recraft-ai
scheme_count: 1
schemes:
- description: Recraft API token issued from the Recraft profile. Sent as `Authorization`.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/recraft-images-api-openapi.yml
  type: http
slug: recraft-ai-authentication
source_filename: recraft-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/recraft-images-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Recraft API token issued from the Recraft profile. Sent as `Authorization`.\n  sources:\n  - openapi/recraft-images-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recraft-ai/refs/heads/main/authentication/recraft-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- Image Generation
- Generative AI
- Vector Graphics
- Brand Design
- Design Tools
- Foundation Models
- MCP
---
