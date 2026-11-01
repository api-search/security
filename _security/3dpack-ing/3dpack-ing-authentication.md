---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: 3dpack-ing-packing-api-openapi.yml
  format: yaml
  label: 3dpack-ing Packing API
  slug: 3dpack-ing-packing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dpack-ing/openapi/3dpack-ing-packing-api-openapi.yml
- filename: 3dpack-ing-typed-api-openapi.yml
  format: yaml
  label: 3dpack-ing Typed API
  slug: 3dpack-ing-typed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dpack-ing/openapi/3dpack-ing-typed-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: 3Dpack Ing Authentication
name_suffix: Authentication
oauth_flows: []
overview: 3dpack-ing secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 3dpack-ing
provider_slug: 3dpack-ing
scheme_count: 2
schemes:
- description: Alternative to sending `apiKey` in the body. `username` is still required alongside it.
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/3dpack-ing-openapi.json
  - openapi/3dpack-ing-original.json
  type: apiKey
- description: The account the key belongs to. Required with X-API-Key on the typed endpoints.
  in: header
  name: apiUsernameHeader
  parameter: X-API-Username
  sources:
  - openapi/3dpack-ing-openapi.json
  - openapi/3dpack-ing-original.json
  type: apiKey
slug: 3dpack-ing-authentication
source_filename: 3dpack-ing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/3dpack-ing-openapi.json, openapi/3dpack-ing-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Alternative to sending `apiKey` in the body. `username` is still required alongside\n    it.\n  sources:\n  - openapi/3dpack-ing-openapi.json\n  - openapi/3dpack-ing-original.json\n- name: apiUsernameHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Username\n  description: The account the key belongs to. Required with X-API-Key on the typed endpoints.\n  sources:\n  - openapi/3dpack-ing-openapi.json\n  - openapi/3dpack-ing-original.json\n"
source_yaml_url: https://artifacts.apis.io/3dpack-ing/authentication/3dpack-ing-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Logistics
- 3D
- API
- SaaS
---
