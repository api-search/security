---
anonymous_access: false
api_key_in: []
api_specs:
- filename: thalium-openapi-generated.yml
  format: yaml
  label: SYSGRAFT API
  slug: thalium-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thalium/openapi/_ae-authored/thalium-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Thalium Authentication
name_suffix: Authentication
oauth_flows: []
overview: SYSGRAFT declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SYSGRAFT
provider_slug: thalium
scheme_count: 1
schemes:
- description: API key with scopes invoke, memory:read, memory:write, memory:admin, audit:read, config:write, admin
  in: header
  name: X-API-Key
  type: apiKey
slug: thalium-authentication
source_filename: thalium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: searched\nsource: https://thalium.io/docs/api\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key with scopes invoke, memory:read, memory:write, memory:admin, audit:read, config:write, admin\n"
source_yaml_url: https://artifacts.apis.io/thalium/authentication/thalium-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Privacy
- Memory API
- Orchestration
---
