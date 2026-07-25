---
api_key_in:
- header
api_specs:
- filename: roblox-engine-api-assets-api-openapi.yml
  format: yaml
  label: Roblox Engine API Assets API
  slug: roblox-engine-api-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/openapi/roblox-engine-api-assets-api-openapi.yml
- filename: roblox-engine-api-data-stores-api-openapi.yml
  format: yaml
  label: Roblox Engine API Data Stores API
  slug: roblox-engine-api-data-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/openapi/roblox-engine-api-data-stores-api-openapi.yml
- filename: roblox-engine-api-groups-api-openapi.yml
  format: yaml
  label: Roblox Engine API Groups API
  slug: roblox-engine-api-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/openapi/roblox-engine-api-groups-api-openapi.yml
- filename: roblox-engine-api-messaging-api-openapi.yml
  format: yaml
  label: Roblox Engine API Messaging API
  slug: roblox-engine-api-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/openapi/roblox-engine-api-messaging-api-openapi.yml
- filename: roblox-engine-api-places-api-openapi.yml
  format: yaml
  label: Roblox Engine API Places API
  slug: roblox-engine-api-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/openapi/roblox-engine-api-places-api-openapi.yml
- filename: roblox-engine-api-universes-api-openapi.yml
  format: yaml
  label: Roblox Engine API Universes API
  slug: roblox-engine-api-universes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/openapi/roblox-engine-api-universes-api-openapi.yml
- filename: roblox-engine-api-users-api-openapi.yml
  format: yaml
  label: Roblox Engine API Users API
  slug: roblox-engine-api-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/openapi/roblox-engine-api-users-api-openapi.yml
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
