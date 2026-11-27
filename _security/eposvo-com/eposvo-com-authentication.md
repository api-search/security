---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eposvo-com-dataset-api-openapi.yml
  format: yaml
  label: Eposvo Dataset API
  slug: eposvo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eposvo-com/openapi/eposvo-com-dataset-api-openapi.yml
- filename: eposvo-com-mcp-api-openapi.yml
  format: yaml
  label: Eposvo MCP API
  slug: eposvo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eposvo-com/openapi/eposvo-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Eposvo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eposvo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eposvo
provider_slug: eposvo-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/app-eposvo-com-openapi.json
  - openapi/eposvo-com-openapi.json
  type: http
slug: eposvo-com-authentication
source_filename: eposvo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/app-eposvo-com-openapi.json, openapi/eposvo-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/app-eposvo-com-openapi.json\n  - openapi/eposvo-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/eposvo-com/authentication/eposvo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- EPOS
- Restaurant
- United Kingdom
- Software-as-a-Service
---
