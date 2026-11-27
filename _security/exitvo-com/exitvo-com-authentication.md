---
anonymous_access: false
api_key_in: []
api_specs:
- filename: exitvo-com-dataset-api-openapi.yml
  format: yaml
  label: Exitvo Dataset API
  slug: exitvo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exitvo-com/openapi/exitvo-com-dataset-api-openapi.yml
- filename: exitvo-com-mcp-api-openapi.yml
  format: yaml
  label: Exitvo MCP API
  slug: exitvo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exitvo-com/openapi/exitvo-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Exitvo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Exitvo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Exitvo
provider_slug: exitvo-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/exitvo-com-openapi.json
  type: http
slug: exitvo-com-authentication
source_filename: exitvo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/exitvo-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/exitvo-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/exitvo-com/authentication/exitvo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Business
- Tools
- Checklist
- Valuation
---
