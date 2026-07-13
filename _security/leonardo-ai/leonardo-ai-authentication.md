---
api_key_in: []
api_specs:
- filename: leonardo-ai-image-generation-openapi.json
  format: json
  label: Leonardo.AI Image Generation API
  slug: leonardo-ai-image-generation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-image-generation-openapi.json
- filename: leonardo-ai-video-generation-openapi.json
  format: json
  label: Leonardo.AI Video Generation API
  slug: leonardo-ai-video-generation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-video-generation-openapi.json
- filename: leonardo-ai-variation-openapi.json
  format: json
  label: Leonardo.AI Variation and Upscale API
  slug: leonardo-ai-variation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-variation-openapi.json
- filename: leonardo-ai-realtime-canvas-openapi.json
  format: json
  label: Leonardo.AI Realtime Canvas API
  slug: leonardo-ai-realtime-canvas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-realtime-canvas-openapi.json
- filename: leonardo-ai-models-openapi.json
  format: json
  label: Leonardo.AI Models API
  slug: leonardo-ai-models
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-models-openapi.json
- filename: leonardo-ai-elements-openapi.json
  format: json
  label: Leonardo.AI Elements API
  slug: leonardo-ai-elements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-elements-openapi.json
- filename: leonardo-ai-datasets-openapi.json
  format: json
  label: Leonardo.AI Datasets API
  slug: leonardo-ai-datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-datasets-openapi.json
- filename: leonardo-ai-init-images-openapi.json
  format: json
  label: Leonardo.AI Init Images API
  slug: leonardo-ai-init-images
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-init-images-openapi.json
- filename: leonardo-ai-media-openapi.json
  format: json
  label: Leonardo.AI Media API
  slug: leonardo-ai-media
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-media-openapi.json
- filename: leonardo-ai-3d-model-assets-openapi.json
  format: json
  label: Leonardo.AI 3D Model Assets API
  slug: leonardo-ai-3d-model-assets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-3d-model-assets-openapi.json
- filename: leonardo-ai-blueprints-openapi.json
  format: json
  label: Leonardo.AI Blueprints API
  slug: leonardo-ai-blueprints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-blueprints-openapi.json
- filename: leonardo-ai-prompt-openapi.json
  format: json
  label: Leonardo.AI Prompt API
  slug: leonardo-ai-prompt
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-prompt-openapi.json
- filename: leonardo-ai-pricing-calculator-openapi.json
  format: json
  label: Leonardo.AI Pricing Calculator API
  slug: leonardo-ai-pricing-calculator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-pricing-calculator-openapi.json
- filename: leonardo-ai-user-openapi.json
  format: json
  label: Leonardo.AI User API
  slug: leonardo-ai-user
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-user-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Leonardo Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leonardo.AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Leonardo.AI
provider_slug: leonardo-ai
scheme_count: 1
schemes:
- bearerFormat: auth-scheme
  description: 'Bearer HTTP authentication. Allowed headers `Authorization: Bearer <api_key>`'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/leonardo-ai-3d-model-assets-openapi.json
  - openapi/leonardo-ai-blueprints-openapi.json
  - openapi/leonardo-ai-datasets-openapi.json
  - openapi/leonardo-ai-elements-openapi.json
  - openapi/leonardo-ai-image-generation-openapi.json
  - openapi/leonardo-ai-init-images-openapi.json
  - openapi/leonardo-ai-media-openapi.json
  - openapi/leonardo-ai-models-openapi.json
  - openapi/leonardo-ai-pricing-calculator-openapi.json
  - openapi/leonardo-ai-prompt-openapi.json
  - openapi/leonardo-ai-realtime-canvas-openapi.json
  - openapi/leonardo-ai-user-openapi.json
  - openapi/leonardo-ai-variation-openapi.json
  - openapi/leonardo-ai-video-generation-openapi.json
  type: http
slug: leonardo-ai-authentication
source_filename: leonardo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/leonardo-ai-3d-model-assets-openapi.json, openapi/leonardo-ai-blueprints-openapi.json,\n  openapi/leonardo-ai-datasets-openapi.json, openapi/leonardo-ai-elements-openapi.json, openapi/leonardo-ai-image-generation-openapi.json,\n  openapi/leonardo-ai-init-images-openapi.json, openapi/leonardo-ai-media-openapi.json, openapi/leonardo-ai-models-openapi.json,\n  openapi/leonardo-ai-pricing-calculator-openapi.json, openapi/leonardo-ai-prompt-openapi.json,\n  openapi/leonardo-ai-realtime-canvas-openapi.json, openapi/leonardo-ai-user-openapi.json ...\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: auth-scheme\n  description: 'Bearer HTTP authentication. Allowed headers `Authorization: Bearer <api_key>`'\n  sources:\n  - openapi/leonardo-ai-3d-model-assets-openapi.json\n  - openapi/leonardo-ai-blueprints-openapi.json\n  - openapi/leonardo-ai-datasets-openapi.json\n\
  \  - openapi/leonardo-ai-elements-openapi.json\n  - openapi/leonardo-ai-image-generation-openapi.json\n  - openapi/leonardo-ai-init-images-openapi.json\n  - openapi/leonardo-ai-media-openapi.json\n  - openapi/leonardo-ai-models-openapi.json\n  - openapi/leonardo-ai-pricing-calculator-openapi.json\n  - openapi/leonardo-ai-prompt-openapi.json\n  - openapi/leonardo-ai-realtime-canvas-openapi.json\n  - openapi/leonardo-ai-user-openapi.json\n  - openapi/leonardo-ai-variation-openapi.json\n  - openapi/leonardo-ai-video-generation-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/authentication/leonardo-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- Image Generation
- Video Generation
- Generative AI
- Creative
- 3D
- Diffusion
- Canva
---
