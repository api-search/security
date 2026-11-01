---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: kreatorflow-ai-audio-api-openapi.yml
  format: yaml
  label: kreatorflow-ai Audio API
  slug: kreatorflow-ai-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kreatorflow-ai/openapi/kreatorflow-ai-audio-api-openapi.yml
- filename: kreatorflow-ai-images-api-openapi.yml
  format: yaml
  label: kreatorflow-ai Images API
  slug: kreatorflow-ai-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kreatorflow-ai/openapi/kreatorflow-ai-images-api-openapi.yml
- filename: kreatorflow-ai-jobs-api-openapi.yml
  format: yaml
  label: kreatorflow-ai Jobs API
  slug: kreatorflow-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kreatorflow-ai/openapi/kreatorflow-ai-jobs-api-openapi.yml
- filename: kreatorflow-ai-lip-sync-api-openapi.yml
  format: yaml
  label: kreatorflow-ai Lip Sync API
  slug: kreatorflow-ai-lip-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kreatorflow-ai/openapi/kreatorflow-ai-lip-sync-api-openapi.yml
- filename: kreatorflow-ai-mcp-api-openapi.yml
  format: yaml
  label: kreatorflow-ai MCP API
  slug: kreatorflow-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kreatorflow-ai/openapi/kreatorflow-ai-mcp-api-openapi.yml
- filename: kreatorflow-ai-models-api-openapi.yml
  format: yaml
  label: kreatorflow-ai Models API
  slug: kreatorflow-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kreatorflow-ai/openapi/kreatorflow-ai-models-api-openapi.yml
- filename: kreatorflow-ai-uploads-api-openapi.yml
  format: yaml
  label: kreatorflow-ai Uploads API
  slug: kreatorflow-ai-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kreatorflow-ai/openapi/kreatorflow-ai-uploads-api-openapi.yml
- filename: kreatorflow-ai-video-api-openapi.yml
  format: yaml
  label: kreatorflow-ai Video API
  slug: kreatorflow-ai-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kreatorflow-ai/openapi/kreatorflow-ai-video-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Kreatorflow Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: kreatorflow-ai secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: kreatorflow-ai
provider_slug: kreatorflow-ai
scheme_count: 2
schemes:
- description: Your KreatorFlow API key (kf_...) as a bearer token. Keep it on your server.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/developers.kreatorflow.ai-openapi.json
  - openapi/kreatorflow-ai-openapi.json
  type: http
- description: Alternative to the Authorization header.
  in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/developers.kreatorflow.ai-openapi.json
  - openapi/kreatorflow-ai-openapi.json
  type: apiKey
slug: kreatorflow-ai-authentication
source_filename: kreatorflow-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/developers.kreatorflow.ai-openapi.json, openapi/kreatorflow-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Your KreatorFlow API key (kf_...) as a bearer token. Keep it on your server.\n  sources:\n  - openapi/developers.kreatorflow.ai-openapi.json\n  - openapi/kreatorflow-ai-openapi.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Alternative to the Authorization header.\n  sources:\n  - openapi/developers.kreatorflow.ai-openapi.json\n  - openapi/kreatorflow-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/kreatorflow-ai/authentication/kreatorflow-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI
- Video
- Image
- Voice
- API
- Platform
---
