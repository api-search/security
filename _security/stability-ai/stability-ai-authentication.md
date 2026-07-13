---
api_key_in: []
api_specs:
- filename: stability-ai-stable-image-generate-openapi.yml
  format: yaml
  label: Stability AI Stable Image Generate API
  slug: stable-image-generate
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-stable-image-generate-openapi.yml
- filename: stability-ai-stable-image-edit-openapi.yml
  format: yaml
  label: Stability AI Stable Image Edit API
  slug: stable-image-edit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-stable-image-edit-openapi.yml
- filename: stability-ai-stable-image-upscale-openapi.yml
  format: yaml
  label: Stability AI Stable Image Upscale API
  slug: stable-image-upscale
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-stable-image-upscale-openapi.yml
- filename: stability-ai-stable-image-control-openapi.yml
  format: yaml
  label: Stability AI Stable Image Control API
  slug: stable-image-control
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-stable-image-control-openapi.yml
- filename: stability-ai-stable-video-diffusion-openapi.yml
  format: yaml
  label: Stability AI Stable Video Diffusion API
  slug: stable-video-diffusion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-stable-video-diffusion-openapi.yml
- filename: stability-ai-stable-fast-3d-openapi.yml
  format: yaml
  label: Stability AI Stable Fast 3D API
  slug: stable-fast-3d
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-stable-fast-3d-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stability Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stability AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stability AI
provider_slug: stability-ai
scheme_count: 1
schemes:
- description: API key authentication. Pass your Stability AI API key as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/stability-ai-stable-fast-3d-openapi.yml
  - openapi/stability-ai-stable-image-control-openapi.yml
  - openapi/stability-ai-stable-image-edit-openapi.yml
  - openapi/stability-ai-stable-image-generate-openapi.yml
  - openapi/stability-ai-stable-image-upscale-openapi.yml
  - openapi/stability-ai-stable-video-diffusion-openapi.yml
  type: http
slug: stability-ai-authentication
source_filename: stability-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stability-ai-stable-fast-3d-openapi.yml, openapi/stability-ai-stable-image-control-openapi.yml,\n  openapi/stability-ai-stable-image-edit-openapi.yml, openapi/stability-ai-stable-image-generate-openapi.yml,\n  openapi/stability-ai-stable-image-upscale-openapi.yml, openapi/stability-ai-stable-video-diffusion-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key authentication. Pass your Stability AI API key as a Bearer token in the\n    Authorization header.\n  sources:\n  - openapi/stability-ai-stable-fast-3d-openapi.yml\n  - openapi/stability-ai-stable-image-control-openapi.yml\n  - openapi/stability-ai-stable-image-edit-openapi.yml\n  - openapi/stability-ai-stable-image-generate-openapi.yml\n  - openapi/stability-ai-stable-image-upscale-openapi.yml\n  - openapi/stability-ai-stable-video-diffusion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/authentication/stability-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- 3D Generation
- AI
- Generative AI
- Image Generation
- Image Editing
- Machine Learning
- Stable Diffusion
- Text to Image
- Video Generation
---
