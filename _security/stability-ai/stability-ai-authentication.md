---
api_key_in: []
api_specs:
- filename: stability-ai-3d-generation-api-openapi.yml
  format: yaml
  label: Stability AI 3D Generation API
  slug: stability-ai-3d-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-3d-generation-api-openapi.yml
- filename: stability-ai-conservative-upscale-api-openapi.yml
  format: yaml
  label: Stability AI Conservative Upscale API
  slug: stability-ai-conservative-upscale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-conservative-upscale-api-openapi.yml
- filename: stability-ai-creative-upscale-api-openapi.yml
  format: yaml
  label: Stability AI Creative Upscale API
  slug: stability-ai-creative-upscale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-creative-upscale-api-openapi.yml
- filename: stability-ai-erase-api-openapi.yml
  format: yaml
  label: Stability AI Erase API
  slug: stability-ai-erase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-erase-api-openapi.yml
- filename: stability-ai-fast-upscale-api-openapi.yml
  format: yaml
  label: Stability AI Fast Upscale API
  slug: stability-ai-fast-upscale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-fast-upscale-api-openapi.yml
- filename: stability-ai-generate-core-api-openapi.yml
  format: yaml
  label: Stability AI Generate Core API
  slug: stability-ai-generate-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-generate-core-api-openapi.yml
- filename: stability-ai-generate-sd3-api-openapi.yml
  format: yaml
  label: Stability AI Generate SD3 API
  slug: stability-ai-generate-sd3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-generate-sd3-api-openapi.yml
- filename: stability-ai-generate-ultra-api-openapi.yml
  format: yaml
  label: Stability AI Generate Ultra API
  slug: stability-ai-generate-ultra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-generate-ultra-api-openapi.yml
- filename: stability-ai-image-to-video-api-openapi.yml
  format: yaml
  label: Stability AI Image to Video API
  slug: stability-ai-image-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-image-to-video-api-openapi.yml
- filename: stability-ai-inpaint-api-openapi.yml
  format: yaml
  label: Stability AI Inpaint API
  slug: stability-ai-inpaint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-inpaint-api-openapi.yml
- filename: stability-ai-outpaint-api-openapi.yml
  format: yaml
  label: Stability AI Outpaint API
  slug: stability-ai-outpaint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-outpaint-api-openapi.yml
- filename: stability-ai-remove-background-api-openapi.yml
  format: yaml
  label: Stability AI Remove Background API
  slug: stability-ai-remove-background-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-remove-background-api-openapi.yml
- filename: stability-ai-replace-background-and-relight-api-openapi.yml
  format: yaml
  label: Stability AI Replace Background and Relight API
  slug: stability-ai-replace-background-and-relight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-replace-background-and-relight-api-openapi.yml
- filename: stability-ai-search-and-recolor-api-openapi.yml
  format: yaml
  label: Stability AI Search and Recolor API
  slug: stability-ai-search-and-recolor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-search-and-recolor-api-openapi.yml
- filename: stability-ai-search-and-replace-api-openapi.yml
  format: yaml
  label: Stability AI Search and Replace API
  slug: stability-ai-search-and-replace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-search-and-replace-api-openapi.yml
- filename: stability-ai-sketch-api-openapi.yml
  format: yaml
  label: Stability AI Sketch API
  slug: stability-ai-sketch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-sketch-api-openapi.yml
- filename: stability-ai-structure-api-openapi.yml
  format: yaml
  label: Stability AI Structure API
  slug: stability-ai-structure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-structure-api-openapi.yml
- filename: stability-ai-style-api-openapi.yml
  format: yaml
  label: Stability AI Style API
  slug: stability-ai-style-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-style-api-openapi.yml
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
