---
anonymous_access: false
api_key_in: []
api_specs:
- filename: krea-ai-assets-api-openapi.yml
  format: yaml
  label: Krea Assets API
  slug: krea-ai-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krea-ai/openapi/krea-ai-assets-api-openapi.yml
- filename: krea-ai-general-api-openapi.yml
  format: yaml
  label: Krea General API
  slug: krea-ai-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krea-ai/openapi/krea-ai-general-api-openapi.yml
- filename: krea-ai-image-api-openapi.yml
  format: yaml
  label: Krea Image API
  slug: krea-ai-image-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krea-ai/openapi/krea-ai-image-api-openapi.yml
- filename: krea-ai-image-enhance-api-openapi.yml
  format: yaml
  label: Krea Image Enhance API
  slug: krea-ai-image-enhance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krea-ai/openapi/krea-ai-image-enhance-api-openapi.yml
- filename: krea-ai-node-apps-api-openapi.yml
  format: yaml
  label: Krea Node Apps API
  slug: krea-ai-node-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krea-ai/openapi/krea-ai-node-apps-api-openapi.yml
- filename: krea-ai-styles-api-openapi.yml
  format: yaml
  label: Krea Styles API
  slug: krea-ai-styles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krea-ai/openapi/krea-ai-styles-api-openapi.yml
- filename: krea-ai-video-api-openapi.yml
  format: yaml
  label: Krea Video API
  slug: krea-ai-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krea-ai/openapi/krea-ai-video-api-openapi.yml
- filename: krea-ai-audio-api-openapi.yml
  format: yaml
  label: Krea Audio API
  slug: krea-ai-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krea-ai/openapi/krea-ai-audio-api-openapi.yml
- filename: krea-ai-krea-api-openapi.yml
  format: yaml
  label: Krea Krea API
  slug: krea-ai-krea-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krea-ai/openapi/krea-ai-krea-api-openapi.yml
- filename: krea-ai-usage-api-openapi.yml
  format: yaml
  label: Krea Usage API
  slug: krea-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krea-ai/openapi/krea-ai-usage-api-openapi.yml
- filename: krea-ai-utilities-api-openapi.yml
  format: yaml
  label: Krea Utilities API
  slug: krea-ai-utilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krea-ai/openapi/krea-ai-utilities-api-openapi.yml
- filename: krea-ai-video-enhance-api-openapi.yml
  format: yaml
  label: Krea Video Enhance API
  slug: krea-ai-video-enhance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krea-ai/openapi/krea-ai-video-enhance-api-openapi.yml
- filename: krea-ai-3-d-api-openapi.yml
  format: yaml
  label: Krea 3 D API
  slug: krea-ai-3-d-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krea-ai/openapi/krea-ai-3-d-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/krea-ai/authentication/krea-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Image Generation
- Video Generation
- Generative AI
- Real-Time
- Multi-Modal
- Creative Tools
- 3D
- Upscaling
---
