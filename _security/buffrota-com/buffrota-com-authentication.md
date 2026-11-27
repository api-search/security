---
anonymous_access: false
api_key_in: []
api_specs:
- filename: buffrota-com-dataset-api-openapi.yml
  format: yaml
  label: Buffrota Dataset API
  slug: buffrota-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buffrota-com/openapi/buffrota-com-dataset-api-openapi.yml
- filename: buffrota-com-enquiry-api-openapi.yml
  format: yaml
  label: Buffrota Enquiry API
  slug: buffrota-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buffrota-com/openapi/buffrota-com-enquiry-api-openapi.yml
- filename: buffrota-com-mcp-api-openapi.yml
  format: yaml
  label: Buffrota MCP API
  slug: buffrota-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buffrota-com/openapi/buffrota-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Buffrota Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buffrota secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Buffrota
provider_slug: buffrota-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/buffrota-com-openapi.json
  type: http
slug: buffrota-com-authentication
source_filename: buffrota-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/buffrota-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/buffrota-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/buffrota-com/authentication/buffrota-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Data
- Cleaning
- Pricing
- US
- Commercial
---
