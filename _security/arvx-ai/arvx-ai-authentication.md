---
anonymous_access: false
api_key_in: []
api_specs:
- filename: arvx-ai-readings-api-openapi.yml
  format: yaml
  label: ARVX Readings API
  slug: arvx-ai-readings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arvx-ai/openapi/arvx-ai-readings-api-openapi.yml
- filename: arvx-ai-records-api-openapi.yml
  format: yaml
  label: ARVX Records API
  slug: arvx-ai-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arvx-ai/openapi/arvx-ai-records-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Arvx Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: ARVX declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ARVX
provider_slug: arvx-ai
scheme_count: 2
schemes:
- description: API key header
  in: header
  name: x-arvx-key
  type: apiKey
- description: Bearer token authentication
  scheme: bearer
  type: http
slug: arvx-ai-authentication
source_filename: arvx-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: https://developer.arvx.ai/openapi.json\nschemes:\n  - type: apiKey\n    name: x-arvx-key\n    in: header\n    description: API key header\n  - type: http\n    scheme: bearer\n    description: Bearer token authentication\n"
source_yaml_url: https://artifacts.apis.io/arvx-ai/authentication/arvx-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
---
