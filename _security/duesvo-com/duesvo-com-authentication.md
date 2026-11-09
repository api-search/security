---
anonymous_access: false
api_key_in: []
api_specs:
- filename: duesvo-com-dataset-api-openapi.yml
  format: yaml
  label: Duesvo Dataset API
  slug: duesvo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duesvo-com/openapi/duesvo-com-dataset-api-openapi.yml
- filename: duesvo-com-mcp-api-openapi.yml
  format: yaml
  label: Duesvo MCP API
  slug: duesvo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duesvo-com/openapi/duesvo-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Duesvo Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Duesvo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Duesvo
provider_slug: duesvo-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/app-duesvo-com-openapi.json
  - openapi/duesvo-com-openapi.json
  type: http
slug: duesvo-com-authentication
source_filename: duesvo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/app-duesvo-com-openapi.json, openapi/duesvo-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/app-duesvo-com-openapi.json\n  - openapi/duesvo-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/duesvo-com/authentication/duesvo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Membership
- Non-Profit
- Clubs
- Associations
- Software
---
