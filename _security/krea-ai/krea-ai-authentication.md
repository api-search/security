---
api_key_in: []
api_specs:
- filename: krea-ai-assets-api-openapi.yml
  format: yaml
  label: Krea Assets API
  slug: krea-ai-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-ai-assets-api-openapi.yml
- filename: krea-ai-general-api-openapi.yml
  format: yaml
  label: Krea General API
  slug: krea-ai-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-ai-general-api-openapi.yml
- filename: krea-ai-image-api-openapi.yml
  format: yaml
  label: Krea Image API
  slug: krea-ai-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-ai-image-api-openapi.yml
- filename: krea-ai-image-enhance-api-openapi.yml
  format: yaml
  label: Krea Image Enhance API
  slug: krea-ai-image-enhance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-ai-image-enhance-api-openapi.yml
- filename: krea-ai-node-apps-api-openapi.yml
  format: yaml
  label: Krea Node Apps API
  slug: krea-ai-node-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-ai-node-apps-api-openapi.yml
- filename: krea-ai-styles-api-openapi.yml
  format: yaml
  label: Krea Styles API
  slug: krea-ai-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-ai-styles-api-openapi.yml
- filename: krea-ai-video-api-openapi.yml
  format: yaml
  label: Krea Video API
  slug: krea-ai-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-ai-video-api-openapi.yml
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
- Artificial Intelligence
- Image-Generation
- Video Generation
- Generative AI
- Real-Time
- Multimodal
- Creative Tools
- 3D
- Upscaling
---
