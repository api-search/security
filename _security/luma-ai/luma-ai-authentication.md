---
api_key_in: []
api_specs:
- filename: luma-ai-callback-asyncapi.yml
  format: yaml
  label: Luma Dream Machine API
  slug: dream-machine
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-ai/refs/heads/main/asyncapi/luma-ai-callback-asyncapi.yml
- filename: luma-ai-concepts-api-openapi.yml
  format: yaml
  label: Luma AI Concepts API
  slug: luma-ai-concepts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-ai/refs/heads/main/openapi/luma-ai-concepts-api-openapi.yml
- filename: luma-ai-credits-api-openapi.yml
  format: yaml
  label: Luma AI Credits API
  slug: luma-ai-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-ai/refs/heads/main/openapi/luma-ai-credits-api-openapi.yml
- filename: luma-ai-generations-api-openapi.yml
  format: yaml
  label: Luma AI Generations API
  slug: luma-ai-generations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-ai/refs/heads/main/openapi/luma-ai-generations-api-openapi.yml
- filename: luma-ai-image-api-openapi.yml
  format: yaml
  label: Luma AI Image API
  slug: luma-ai-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-ai/refs/heads/main/openapi/luma-ai-image-api-openapi.yml
- filename: luma-ai-system-api-openapi.yml
  format: yaml
  label: Luma AI System API
  slug: luma-ai-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-ai/refs/heads/main/openapi/luma-ai-system-api-openapi.yml
- filename: luma-ai-video-api-openapi.yml
  format: yaml
  label: Luma AI Video API
  slug: luma-ai-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-ai/refs/heads/main/openapi/luma-ai-video-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Luma Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Luma AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Luma AI
provider_slug: luma-ai
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/luma-ai-openapi.yml
  type: http
slug: luma-ai-authentication
source_filename: luma-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/luma-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/luma-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luma-ai/refs/heads/main/authentication/luma-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Video Generation
- Image-Generation
- 3D
- Dream Machine
- Multimodal
---
