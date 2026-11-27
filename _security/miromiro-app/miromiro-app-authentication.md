---
anonymous_access: false
api_key_in: []
api_specs:
- filename: miromiro-app-account-api-openapi.yml
  format: yaml
  label: MiroMiro Account API
  slug: miromiro-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/miromiro-app/openapi/miromiro-app-account-api-openapi.yml
- filename: miromiro-app-audio-api-openapi.yml
  format: yaml
  label: MiroMiro Audio API
  slug: miromiro-app-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/miromiro-app/openapi/miromiro-app-audio-api-openapi.yml
- filename: miromiro-app-brand-api-openapi.yml
  format: yaml
  label: MiroMiro Brand API
  slug: miromiro-app-brand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/miromiro-app/openapi/miromiro-app-brand-api-openapi.yml
- filename: miromiro-app-code-api-openapi.yml
  format: yaml
  label: MiroMiro Code API
  slug: miromiro-app-code-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/miromiro-app/openapi/miromiro-app-code-api-openapi.yml
- filename: miromiro-app-extract-api-openapi.yml
  format: yaml
  label: MiroMiro Extract API
  slug: miromiro-app-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/miromiro-app/openapi/miromiro-app-extract-api-openapi.yml
- filename: miromiro-app-fonts-api-openapi.yml
  format: yaml
  label: MiroMiro Fonts API
  slug: miromiro-app-fonts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/miromiro-app/openapi/miromiro-app-fonts-api-openapi.yml
- filename: miromiro-app-images-api-openapi.yml
  format: yaml
  label: MiroMiro Images API
  slug: miromiro-app-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/miromiro-app/openapi/miromiro-app-images-api-openapi.yml
- filename: miromiro-app-lottie-api-openapi.yml
  format: yaml
  label: MiroMiro Lottie API
  slug: miromiro-app-lottie-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/miromiro-app/openapi/miromiro-app-lottie-api-openapi.yml
- filename: miromiro-app-site-api-openapi.yml
  format: yaml
  label: MiroMiro Site API
  slug: miromiro-app-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/miromiro-app/openapi/miromiro-app-site-api-openapi.yml
- filename: miromiro-app-svg-api-openapi.yml
  format: yaml
  label: MiroMiro Svg API
  slug: miromiro-app-svg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/miromiro-app/openapi/miromiro-app-svg-api-openapi.yml
- filename: miromiro-app-videos-api-openapi.yml
  format: yaml
  label: MiroMiro Videos API
  slug: miromiro-app-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/miromiro-app/openapi/miromiro-app-videos-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: MiroMiro Authentication
name_suffix: Authentication
oauth_flows: []
overview: MiroMiro secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MiroMiro
provider_slug: miromiro-app
scheme_count: 1
schemes:
- description: 'API key from the MiroMiro console, format mm_live_… Sent as `Authorization: Bearer mm_live_…`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/miromiro-app-openapi.json
  type: http
slug: miromiro-app-authentication
source_filename: miromiro-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/miromiro-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key from the MiroMiro console, format mm_live_… Sent as `Authorization:\n    Bearer mm_live_…`.'\n  sources:\n  - openapi/miromiro-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/miromiro-app/authentication/miromiro-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Design
- Code Generation
- No-Code
- Platform
---
