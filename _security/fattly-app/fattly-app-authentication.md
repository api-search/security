---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fattly-app-account-api-openapi.yml
  format: yaml
  label: Fattly AI Account API
  slug: fattly-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fattly-app/openapi/fattly-app-account-api-openapi.yml
- filename: fattly-app-ad-studio-api-openapi.yml
  format: yaml
  label: Fattly AI Ad Studio API
  slug: fattly-app-ad-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fattly-app/openapi/fattly-app-ad-studio-api-openapi.yml
- filename: fattly-app-audio-api-openapi.yml
  format: yaml
  label: Fattly AI Audio API
  slug: fattly-app-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fattly-app/openapi/fattly-app-audio-api-openapi.yml
- filename: fattly-app-images-api-openapi.yml
  format: yaml
  label: Fattly AI Images API
  slug: fattly-app-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fattly-app/openapi/fattly-app-images-api-openapi.yml
- filename: fattly-app-video-api-openapi.yml
  format: yaml
  label: Fattly AI Video API
  slug: fattly-app-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fattly-app/openapi/fattly-app-video-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fattly AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fattly AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fattly AI
provider_slug: fattly-app
scheme_count: 1
schemes:
- description: API key gpx_live_... from fattly.app → Dashboard → API keys.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fattly-app-openapi.json
  type: http
slug: fattly-app-authentication
source_filename: fattly-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/fattly-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key gpx_live_... from fattly.app → Dashboard → API keys.\n  sources:\n  - openapi/fattly-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fattly-app/authentication/fattly-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Image Generation
- Video Generation
- Marketing
- Content Creation
---
