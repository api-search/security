---
api_key_in: []
api_specs:
- filename: vidgrid-caption-api-openapi.yml
  format: yaml
  label: VidGrid Caption API
  slug: vidgrid-caption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-caption-api-openapi.yml
- filename: vidgrid-folder-api-openapi.yml
  format: yaml
  label: VidGrid Folder API
  slug: vidgrid-folder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-folder-api-openapi.yml
- filename: vidgrid-search-api-openapi.yml
  format: yaml
  label: VidGrid Search API
  slug: vidgrid-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-search-api-openapi.yml
- filename: vidgrid-token-api-openapi.yml
  format: yaml
  label: VidGrid Token API
  slug: vidgrid-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-token-api-openapi.yml
- filename: vidgrid-user-api-openapi.yml
  format: yaml
  label: VidGrid User API
  slug: vidgrid-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-user-api-openapi.yml
- filename: vidgrid-video-api-openapi.yml
  format: yaml
  label: VidGrid Video API
  slug: vidgrid-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-video-api-openapi.yml
- filename: vidgrid-webhooks-api-openapi.yml
  format: yaml
  label: VidGrid Webhooks API
  slug: vidgrid-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Vidgrid Authentication
name_suffix: Authentication
oauth_flows: []
overview: VidGrid secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VidGrid
provider_slug: vidgrid
scheme_count: 2
schemes:
- description: Bearer Authorization
  name: bearer
  scheme: bearer
  sources:
  - openapi/vidgrid-openapi-original.json
  type: http
- description: Where `username` and `password` are api `key` and `secret`
  name: basic
  scheme: basic
  sources:
  - openapi/vidgrid-openapi-original.json
  type: http
slug: vidgrid-authentication
source_filename: vidgrid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/vidgrid-openapi-original.json\ndocs: https://developer.vidgrid.com/docs/v2/\nsummary:\n  types:\n  - http\n  primary: HTTP Basic — API key as username, API secret as password, base64-encoded in the Authorization header\n  key_management: https://app.vidgrid.com/integrations\n  availability: API keys are available during a 14-day trial and restricted to Enterprise accounts afterward.\n  key_types: User keys (individual accounts) and Organization keys (organizational accounts) — documented in the v1 reference.\n  client_side: Keys give full permissions to manage account content and must NEVER be exposed client side; mint record/upload tokens (POST /vidgrid/v2/tokens) for client-side capture flows.\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Bearer Authorization\n  sources:\n  - openapi/vidgrid-openapi-original.json\n- name: basic\n  type: http\n  scheme: basic\n  description: Where `username`\
  \ and `password` are api `key` and `secret`\n  sources:\n  - openapi/vidgrid-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/authentication/vidgrid-authentication.yml
summary_line: http · 2 schemes
tags:
- Video
- Screen Recording
- Captions
- Video Hosting
- Webhook
- Training
- HR
---
