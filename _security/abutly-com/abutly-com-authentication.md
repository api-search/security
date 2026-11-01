---
anonymous_access: false
api_key_in: []
api_specs:
- filename: abutly-com-dataset-api-openapi.yml
  format: yaml
  label: abutly-com Dataset API
  slug: abutly-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abutly-com/openapi/abutly-com-dataset-api-openapi.yml
- filename: abutly-com-mcp-api-openapi.yml
  format: yaml
  label: abutly-com MCP API
  slug: abutly-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abutly-com/openapi/abutly-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Abutly Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: abutly-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: abutly-com
provider_slug: abutly-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/abutly-com-openapi.json
  - openapi/app-abutly-com-openapi.json
  type: http
slug: abutly-com-authentication
source_filename: abutly-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/abutly-com-openapi.json, openapi/app-abutly-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/abutly-com-openapi.json\n  - openapi/app-abutly-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/abutly-com/authentication/abutly-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Construction
- LegalTech
- PartyWall
- UK
---
