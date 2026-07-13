---
api_key_in: []
api_specs:
- filename: krea-api-openapi.json
  format: json
  label: Krea API
  slug: krea-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-api-openapi.json
- filename: krea-api-openapi.json
  format: json
  label: Krea Image Generation API
  slug: krea-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-api-openapi.json
- filename: krea-api-openapi.json
  format: json
  label: Krea Video Generation API
  slug: krea-video-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-api-openapi.json
- filename: krea-api-openapi.json
  format: json
  label: Krea Image Enhance API
  slug: krea-image-enhance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-api-openapi.json
- filename: krea-api-openapi.json
  format: json
  label: Krea Styles API (LoRA)
  slug: krea-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-api-openapi.json
- filename: krea-api-openapi.json
  format: json
  label: Krea Assets API
  slug: krea-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-api-openapi.json
- filename: krea-api-openapi.json
  format: json
  label: Krea Jobs API
  slug: krea-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-api-openapi.json
- filename: krea-api-openapi.json
  format: json
  label: Krea Node Apps API
  slug: krea-node-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Krea Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Krea secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Krea
provider_slug: krea-ai
scheme_count: 1
schemes:
- bearerFormat: Bearer
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/krea-api-openapi.json
  type: http
slug: krea-ai-authentication
source_filename: krea-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/krea-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Bearer\n  sources:\n  - openapi/krea-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/authentication/krea-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- Image Generation
- Video Generation
- Generative AI
- Real Time
- Multimodal
- Creative Tools
- 3D
- Upscaling
---
