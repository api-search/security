---
anonymous_access: false
api_key_in: []
api_specs:
- filename: extinvo-com-dataset-api-openapi.yml
  format: yaml
  label: Extinvo Dataset API
  slug: extinvo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/extinvo-com/openapi/extinvo-com-dataset-api-openapi.yml
- filename: extinvo-com-mcp-api-openapi.yml
  format: yaml
  label: Extinvo MCP API
  slug: extinvo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/extinvo-com/openapi/extinvo-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Extinvo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Extinvo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Extinvo
provider_slug: extinvo-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/extinvo-com-openapi.json
  type: http
slug: extinvo-com-authentication
source_filename: extinvo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/extinvo-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/extinvo-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/extinvo-com/authentication/extinvo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fire Safety
- Inspection
- Software
- Tools
---
