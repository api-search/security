---
api_key_in:
- header
api_specs:
- filename: argil-openapi.yml
  format: yaml
  label: Argil Videos API
  slug: argil-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argil/refs/heads/main/openapi/argil-openapi.yml
- filename: argil-openapi.yml
  format: yaml
  label: Argil Avatars API
  slug: argil-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argil/refs/heads/main/openapi/argil-openapi.yml
- filename: argil-openapi.yml
  format: yaml
  label: Argil Voices API
  slug: argil-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argil/refs/heads/main/openapi/argil-openapi.yml
- filename: argil-openapi.yml
  format: yaml
  label: Argil Assets API
  slug: argil-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argil/refs/heads/main/openapi/argil-openapi.yml
- filename: argil-openapi.yml
  format: yaml
  label: Argil Webhooks API
  slug: argil-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argil/refs/heads/main/openapi/argil-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Argil Authentication
name_suffix: Authentication
oauth_flows: []
overview: Argil secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Argil
provider_slug: argil
scheme_count: 1
schemes:
- description: API key issued in the Argil dashboard.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/argil-openapi.yml
  type: apiKey
slug: argil-authentication
source_filename: argil-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/argil-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key issued in the Argil dashboard.\n  sources:\n  - openapi/argil-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argil/refs/heads/main/authentication/argil-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Video Generation
- Avatars
- Voice Cloning
- Content Automation
---
