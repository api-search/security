---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cmmsly-com-dataset-api-openapi.yml
  format: yaml
  label: cmmsly-com Dataset API
  slug: cmmsly-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cmmsly-com/openapi/cmmsly-com-dataset-api-openapi.yml
- filename: cmmsly-com-mcp-api-openapi.yml
  format: yaml
  label: cmmsly-com MCP API
  slug: cmmsly-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cmmsly-com/openapi/cmmsly-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cmmsly Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: cmmsly-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: cmmsly-com
provider_slug: cmmsly-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/app-cmmsly-com-openapi.json
  - openapi/cmmsly-com-openapi.json
  type: http
slug: cmmsly-com-authentication
source_filename: cmmsly-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/app-cmmsly-com-openapi.json, openapi/cmmsly-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/app-cmmsly-com-openapi.json\n  - openapi/cmmsly-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cmmsly-com/authentication/cmmsly-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- CMMS
- Maintenance
- Equipment
- Software
- Tools
---
