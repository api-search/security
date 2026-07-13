---
api_key_in:
- header
api_specs:
- filename: sync-labs-openapi.yml
  format: yaml
  label: Sync Labs API
  slug: sync-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sync-labs/refs/heads/main/openapi/sync-labs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sync Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sync Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sync Labs
provider_slug: sync-labs
scheme_count: 1
schemes:
- description: API key from https://sync.so/settings/api-keys
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/sync-labs-openapi.yml
  type: apiKey
slug: sync-labs-authentication
source_filename: sync-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sync-labs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key from https://sync.so/settings/api-keys\n  sources:\n  - openapi/sync-labs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sync-labs/refs/heads/main/authentication/sync-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Content Localization
- Dubbing
- Lip Sync
- Media
- Video
- Visual AI
---
