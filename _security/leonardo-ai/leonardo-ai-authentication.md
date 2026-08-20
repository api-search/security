---
api_key_in: []
api_specs:
- filename: leonardo-ai-3d-model-assets-api-openapi.yml
  format: yaml
  label: Leonardo.AI 3D Model Assets API
  slug: leonardo-ai-3d-model-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-3d-model-assets-api-openapi.yml
- filename: leonardo-ai-blueprints-api-openapi.yml
  format: yaml
  label: Leonardo.AI Blueprints API
  slug: leonardo-ai-blueprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-blueprints-api-openapi.yml
- filename: leonardo-ai-dataset-api-openapi.yml
  format: yaml
  label: Leonardo.AI Dataset API
  slug: leonardo-ai-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-dataset-api-openapi.yml
- filename: leonardo-ai-elements-api-openapi.yml
  format: yaml
  label: Leonardo.AI Elements API
  slug: leonardo-ai-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-elements-api-openapi.yml
- filename: leonardo-ai-image-api-openapi.yml
  format: yaml
  label: Leonardo.AI Image API
  slug: leonardo-ai-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-image-api-openapi.yml
- filename: leonardo-ai-init-images-api-openapi.yml
  format: yaml
  label: Leonardo.AI Init Images API
  slug: leonardo-ai-init-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-init-images-api-openapi.yml
- filename: leonardo-ai-media-api-openapi.yml
  format: yaml
  label: Leonardo.AI Media API
  slug: leonardo-ai-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-media-api-openapi.yml
- filename: leonardo-ai-models-api-openapi.yml
  format: yaml
  label: Leonardo.AI Models API
  slug: leonardo-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-models-api-openapi.yml
- filename: leonardo-ai-motion-api-openapi.yml
  format: yaml
  label: Leonardo.AI Motion API
  slug: leonardo-ai-motion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-motion-api-openapi.yml
- filename: leonardo-ai-pricing-calculator-api-openapi.yml
  format: yaml
  label: Leonardo.AI Pricing Calculator API
  slug: leonardo-ai-pricing-calculator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-pricing-calculator-api-openapi.yml
- filename: leonardo-ai-prompt-api-openapi.yml
  format: yaml
  label: Leonardo.AI Prompt API
  slug: leonardo-ai-prompt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-prompt-api-openapi.yml
- filename: leonardo-ai-realtime-canvas-api-openapi.yml
  format: yaml
  label: Leonardo.AI Realtime Canvas API
  slug: leonardo-ai-realtime-canvas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-realtime-canvas-api-openapi.yml
- filename: leonardo-ai-user-api-openapi.yml
  format: yaml
  label: Leonardo.AI User API
  slug: leonardo-ai-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-user-api-openapi.yml
- filename: leonardo-ai-variation-api-openapi.yml
  format: yaml
  label: Leonardo.AI Variation API
  slug: leonardo-ai-variation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-variation-api-openapi.yml
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
- Artificial Intelligence
- Image-Generation
- Video Generation
- Generative AI
- Creative
- 3D
- Diffusion
- Canva
---
