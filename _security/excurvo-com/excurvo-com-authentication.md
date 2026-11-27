---
anonymous_access: false
api_key_in: []
api_specs:
- filename: excurvo-com-dataset-api-openapi.yml
  format: yaml
  label: Excurvo Dataset API
  slug: excurvo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/excurvo-com/openapi/excurvo-com-dataset-api-openapi.yml
- filename: excurvo-com-mcp-api-openapi.yml
  format: yaml
  label: Excurvo MCP API
  slug: excurvo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/excurvo-com/openapi/excurvo-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Excurvo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Excurvo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Excurvo
provider_slug: excurvo-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/excurvo-com-openapi.json
  type: http
slug: excurvo-com-authentication
source_filename: excurvo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/excurvo-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/excurvo-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/excurvo-com/authentication/excurvo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Travel
- Booking
- Software-as-a-Service
- Tours
- Tools
---
