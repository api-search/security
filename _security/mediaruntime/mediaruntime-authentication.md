---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: mediaruntime-discovery-api-openapi.yml
  format: yaml
  label: MediaRuntime Discovery API
  slug: mediaruntime-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-discovery-api-openapi.yml
- filename: mediaruntime-job-results-api-openapi.yml
  format: yaml
  label: MediaRuntime Job Results API
  slug: mediaruntime-job-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-job-results-api-openapi.yml
- filename: mediaruntime-jobs-api-openapi.yml
  format: yaml
  label: MediaRuntime Jobs API
  slug: mediaruntime-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-jobs-api-openapi.yml
- filename: mediaruntime-media-analysis-api-openapi.yml
  format: yaml
  label: MediaRuntime Media Analysis API
  slug: mediaruntime-media-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-media-analysis-api-openapi.yml
- filename: mediaruntime-mediaruntime-api-api-openapi.yml
  format: yaml
  label: MediaRuntime API
  slug: mediaruntime-mediaruntime-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-mediaruntime-api-api-openapi.yml
- filename: mediaruntime-moderation-api-openapi.yml
  format: yaml
  label: MediaRuntime Moderation API
  slug: mediaruntime-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-moderation-api-openapi.yml
- filename: mediaruntime-recipes-api-openapi.yml
  format: yaml
  label: MediaRuntime Recipes API
  slug: mediaruntime-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-recipes-api-openapi.yml
- filename: mediaruntime-sandbox-api-openapi.yml
  format: yaml
  label: MediaRuntime Sandbox API
  slug: mediaruntime-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-sandbox-api-openapi.yml
- filename: mediaruntime-uploads-api-openapi.yml
  format: yaml
  label: MediaRuntime Uploads API
  slug: mediaruntime-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-uploads-api-openapi.yml
- filename: mediaruntime-watermarks-api-openapi.yml
  format: yaml
  label: MediaRuntime Watermarks API
  slug: mediaruntime-watermarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-watermarks-api-openapi.yml
- filename: mediaruntime-webhooks-api-openapi.yml
  format: yaml
  label: MediaRuntime Webhooks API
  slug: mediaruntime-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-webhooks-api-openapi.yml
- filename: mediaruntime-marketplace-api-openapi.yml
  format: yaml
  label: MediaRuntime Marketplace API
  slug: mediaruntime-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-marketplace-api-openapi.yml
- filename: mediaruntime-sticker-collections-api-openapi.yml
  format: yaml
  label: MediaRuntime Sticker Collections API
  slug: mediaruntime-sticker-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-sticker-collections-api-openapi.yml
- filename: mediaruntime-sticker-runtime-api-openapi.yml
  format: yaml
  label: MediaRuntime Sticker Runtime API
  slug: mediaruntime-sticker-runtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-sticker-runtime-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Mediaruntime Authentication
name_suffix: Authentication
oauth_flows: []
overview: MediaRuntime secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MediaRuntime
provider_slug: mediaruntime
scheme_count: 3
schemes:
- description: MediaRuntime server-side API key. Keep it in a secret manager and never expose it in browser or mobile code.
  in: header
  name: ProductionApiKey
  parameter: X-API-Key
  sources:
  - openapi/mediaruntime-discovery-api-openapi.yml
  - openapi/mediaruntime-job-results-api-openapi.yml
  - openapi/mediaruntime-jobs-api-openapi.yml
  - openapi/mediaruntime-media-analysis-api-openapi.yml
  - openapi/mediaruntime-mediaruntime-api-api-openapi.yml
  - openapi/mediaruntime-moderation-api-openapi.yml
  - openapi/mediaruntime-openapi.json
  - openapi/mediaruntime-recipes-api-openapi.yml
  - openapi/mediaruntime-sandbox-api-openapi.yml
  - openapi/mediaruntime-uploads-api-openapi.yml
  - openapi/mediaruntime-watermarks-api-openapi.yml
  - openapi/mediaruntime-webhooks-api-openapi.yml
  type: apiKey
- description: Ephemeral credential returned by POST /v1/sandbox/session for bounded sandbox jobs only.
  in: header
  name: SandboxToken
  parameter: X-Sandbox-Token
  sources:
  - openapi/mediaruntime-discovery-api-openapi.yml
  - openapi/mediaruntime-job-results-api-openapi.yml
  - openapi/mediaruntime-jobs-api-openapi.yml
  - openapi/mediaruntime-media-analysis-api-openapi.yml
  - openapi/mediaruntime-mediaruntime-api-api-openapi.yml
  - openapi/mediaruntime-moderation-api-openapi.yml
  - openapi/mediaruntime-openapi.json
  - openapi/mediaruntime-recipes-api-openapi.yml
  - openapi/mediaruntime-sandbox-api-openapi.yml
  - openapi/mediaruntime-uploads-api-openapi.yml
  - openapi/mediaruntime-watermarks-api-openapi.yml
  - openapi/mediaruntime-webhooks-api-openapi.yml
  type: apiKey
- bearerFormat: mrt_v1
  description: Short-lived token restricted to one sticker collection and an explicit runtime-operation allowlist.
  name: StickerClientToken
  scheme: bearer
  sources:
  - openapi/mediaruntime-openapi.json
  type: http
slug: mediaruntime-authentication
source_filename: mediaruntime-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: derived\nsource: openapi/mediaruntime-discovery-api-openapi.yml, openapi/mediaruntime-job-results-api-openapi.yml,\n  openapi/mediaruntime-jobs-api-openapi.yml, openapi/mediaruntime-media-analysis-api-openapi.yml,\n  openapi/mediaruntime-mediaruntime-api-api-openapi.yml, openapi/mediaruntime-moderation-api-openapi.yml,\n  openapi/mediaruntime-openapi.json, openapi/mediaruntime-recipes-api-openapi.yml, openapi/mediaruntime-sandbox-api-openapi.yml,\n  openapi/mediaruntime-uploads-api-openapi.yml, openapi/mediaruntime-watermarks-api-openapi.yml,\n  openapi/mediaruntime-webhooks-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ProductionApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: MediaRuntime server-side API key. Keep it in a secret manager and never expose\n    it in browser or mobile code.\n  sources:\n  - openapi/mediaruntime-discovery-api-openapi.yml\n  -\
  \ openapi/mediaruntime-job-results-api-openapi.yml\n  - openapi/mediaruntime-jobs-api-openapi.yml\n  - openapi/mediaruntime-media-analysis-api-openapi.yml\n  - openapi/mediaruntime-mediaruntime-api-api-openapi.yml\n  - openapi/mediaruntime-moderation-api-openapi.yml\n  - openapi/mediaruntime-openapi.json\n  - openapi/mediaruntime-recipes-api-openapi.yml\n  - openapi/mediaruntime-sandbox-api-openapi.yml\n  - openapi/mediaruntime-uploads-api-openapi.yml\n  - openapi/mediaruntime-watermarks-api-openapi.yml\n  - openapi/mediaruntime-webhooks-api-openapi.yml\n- name: SandboxToken\n  type: apiKey\n  in: header\n  parameter: X-Sandbox-Token\n  description: Ephemeral credential returned by POST /v1/sandbox/session for bounded sandbox\n    jobs only.\n  sources:\n  - openapi/mediaruntime-discovery-api-openapi.yml\n  - openapi/mediaruntime-job-results-api-openapi.yml\n  - openapi/mediaruntime-jobs-api-openapi.yml\n  - openapi/mediaruntime-media-analysis-api-openapi.yml\n  - openapi/mediaruntime-mediaruntime-api-api-openapi.yml\n\
  \  - openapi/mediaruntime-moderation-api-openapi.yml\n  - openapi/mediaruntime-openapi.json\n  - openapi/mediaruntime-recipes-api-openapi.yml\n  - openapi/mediaruntime-sandbox-api-openapi.yml\n  - openapi/mediaruntime-uploads-api-openapi.yml\n  - openapi/mediaruntime-watermarks-api-openapi.yml\n  - openapi/mediaruntime-webhooks-api-openapi.yml\n- name: StickerClientToken\n  type: http\n  scheme: bearer\n  bearerFormat: mrt_v1\n  description: Short-lived token restricted to one sticker collection and an explicit runtime-operation\n    allowlist.\n  sources:\n  - openapi/mediaruntime-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/authentication/mediaruntime-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Media Processing
- Video
- Audio
- Runtime
- Video Encoding
- Audio Processing
- Image Processing
- Content Moderation
- Media API
- Asynchronous Processing
---
