---
api_key_in:
- header
api_specs:
- filename: synthesia-assets-api-openapi.yml
  format: yaml
  label: Synthesia Assets API
  slug: synthesia-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthesia/refs/heads/main/openapi/synthesia-assets-api-openapi.yml
- filename: synthesia-auditlogs-api-openapi.yml
  format: yaml
  label: Synthesia AuditLogs API
  slug: synthesia-auditlogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthesia/refs/heads/main/openapi/synthesia-auditlogs-api-openapi.yml
- filename: synthesia-dubbing-api-openapi.yml
  format: yaml
  label: Synthesia Dubbing API
  slug: synthesia-dubbing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthesia/refs/heads/main/openapi/synthesia-dubbing-api-openapi.yml
- filename: synthesia-templates-api-openapi.yml
  format: yaml
  label: Synthesia Templates API
  slug: synthesia-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthesia/refs/heads/main/openapi/synthesia-templates-api-openapi.yml
- filename: synthesia-translations-api-openapi.yml
  format: yaml
  label: Synthesia Translations API
  slug: synthesia-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthesia/refs/heads/main/openapi/synthesia-translations-api-openapi.yml
- filename: synthesia-videos-api-openapi.yml
  format: yaml
  label: Synthesia Videos API
  slug: synthesia-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthesia/refs/heads/main/openapi/synthesia-videos-api-openapi.yml
- filename: synthesia-webhooks-api-openapi.yml
  format: yaml
  label: Synthesia Webhooks API
  slug: synthesia-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthesia/refs/heads/main/openapi/synthesia-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Synthesia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synthesia secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Synthesia
provider_slug: synthesia
scheme_count: 1
schemes:
- description: API key from the Synthesia dashboard, passed in the Authorization header on each request.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/synthesia-openapi.yml
  type: apiKey
slug: synthesia-authentication
source_filename: synthesia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/synthesia-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key from the Synthesia dashboard, passed in the Authorization header on each\n    request.\n  sources:\n  - openapi/synthesia-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthesia/refs/heads/main/authentication/synthesia-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Generative AI
- Video
- Avatars
- Text To Video
- Voices
- Dubbing
- Translation
- Templates
- Enterprise
- Learning
---
