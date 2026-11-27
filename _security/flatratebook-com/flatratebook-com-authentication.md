---
anonymous_access: false
api_key_in: []
api_specs:
- filename: flatratebook-com-dataset-api-openapi.yml
  format: yaml
  label: FlatRateBook Dataset API
  slug: flatratebook-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flatratebook-com/openapi/flatratebook-com-dataset-api-openapi.yml
- filename: flatratebook-com-mcp-api-openapi.yml
  format: yaml
  label: FlatRateBook MCP API
  slug: flatratebook-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flatratebook-com/openapi/flatratebook-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: FlatRateBook Authentication
name_suffix: Authentication
oauth_flows: []
overview: FlatRateBook secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FlatRateBook
provider_slug: flatratebook-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/app-flatratebook-com-openapi.json
  - openapi/flatratebook-com-openapi.json
  type: http
slug: flatratebook-com-authentication
source_filename: flatratebook-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/app-flatratebook-com-openapi.json, openapi/flatratebook-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/app-flatratebook-com-openapi.json\n  - openapi/flatratebook-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/flatratebook-com/authentication/flatratebook-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Field Service Management
- Pricing
- Invoicing
- Calculator
- Small Business
---
