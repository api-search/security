---
api_key_in:
- header
api_specs:
- filename: openapi
  format: yaml
  label: Roblox Open Cloud API
  slug: roblox-open-cloud-api
  spec_type: OpenAPI
  url: https://create.roblox.com/docs/cloud/reference/openapi
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Roblox Engine Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Roblox Engine API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Roblox Engine API
provider_slug: roblox-engine-api
scheme_count: 1
schemes:
- description: Roblox Open Cloud API key scoped to specific resources
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/roblox-open-cloud-openapi.yml
  type: apiKey
slug: roblox-engine-api-authentication
source_filename: roblox-engine-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/roblox-open-cloud-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Roblox Open Cloud API key scoped to specific resources\n  sources:\n  - openapi/roblox-open-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/authentication/roblox-engine-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Gaming
- Game Development
- Metaverse
- Roblox
- Open Cloud
---
