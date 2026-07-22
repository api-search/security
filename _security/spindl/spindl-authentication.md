---
api_key_in:
- header
api_specs:
- filename: spindl-openapi.yml
  format: yaml
  label: Spindl Server-to-Server API
  slug: spindl-server-to-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spindl/refs/heads/main/openapi/spindl-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Spindl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spindl secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spindl
provider_slug: spindl
scheme_count: 1
schemes:
- description: Server-to-Server API key generated on the Settings page in the Spindl app (https://app.spindl.xyz/settings). Distinct from the client-side SDK key.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/spindl-openapi.yml
  type: apiKey
slug: spindl-authentication
source_filename: spindl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/spindl-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Server-to-Server API key generated on the Settings page in the Spindl app (https://app.spindl.xyz/settings).\n    Distinct from the client-side SDK key.\n  sources:\n  - openapi/spindl-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spindl/refs/heads/main/authentication/spindl-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Crypto Web3
- Attribution
- Analytics
- Marketing
- Growth
- SDK
- Web3
---
