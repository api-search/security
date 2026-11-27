---
anonymous_access: false
api_key_in: []
api_specs:
- filename: faktry-ai-audio-api-openapi.yml
  format: yaml
  label: faktry Audio API
  slug: faktry-ai-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faktry-ai/openapi/faktry-ai-audio-api-openapi.yml
- filename: faktry-ai-image-api-openapi.yml
  format: yaml
  label: faktry Image API
  slug: faktry-ai-image-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faktry-ai/openapi/faktry-ai-image-api-openapi.yml
- filename: faktry-ai-pdf-api-openapi.yml
  format: yaml
  label: faktry PDF API
  slug: faktry-ai-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faktry-ai/openapi/faktry-ai-pdf-api-openapi.yml
- filename: faktry-ai-video-api-openapi.yml
  format: yaml
  label: faktry Video API
  slug: faktry-ai-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faktry-ai/openapi/faktry-ai-video-api-openapi.yml
- filename: faktry-ai-3-d-api-openapi.yml
  format: yaml
  label: faktry 3 D API
  slug: faktry-ai-3-d-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faktry-ai/openapi/faktry-ai-3-d-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: faktry Authentication
name_suffix: Authentication
oauth_flows: []
overview: faktry declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: faktry
provider_slug: faktry-ai
scheme_count: 1
schemes:
- bearerFormat: mt_<api-key> | supabase-jwt
  description: 'Pass either an mt_-prefixed API key or a Supabase session JWT as the Bearer token. Example: `Authorization: Bearer mt_abc123...`'
  scheme: bearer
  type: http
slug: faktry-ai-authentication
source_filename: faktry-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://faktry.ai/api/docs/openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: \"mt_<api-key> | supabase-jwt\"\n    description: \"Pass either an mt_-prefixed API key or a Supabase session JWT as the Bearer token. Example: `Authorization: Bearer mt_abc123...`\"\n"
source_yaml_url: https://artifacts.apis.io/faktry-ai/authentication/faktry-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Media
- Platform
- Software-as-a-Service
- Image
- Video
- Audio
- 3D
---
