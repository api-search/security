---
anonymous_access: false
api_key_in: []
api_specs:
- filename: csatzo-com-dataset-api-openapi.yml
  format: yaml
  label: Csatzo Dataset API
  slug: csatzo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csatzo-com/openapi/csatzo-com-dataset-api-openapi.yml
- filename: csatzo-com-mcp-api-openapi.yml
  format: yaml
  label: Csatzo MCP API
  slug: csatzo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csatzo-com/openapi/csatzo-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Csatzo Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Csatzo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Csatzo
provider_slug: csatzo-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/app-csatzo-com-openapi.json
  - openapi/csatzo-com-openapi.json
  type: http
slug: csatzo-com-authentication
source_filename: csatzo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/app-csatzo-com-openapi.json, openapi/csatzo-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/app-csatzo-com-openapi.json\n  - openapi/csatzo-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/csatzo-com/authentication/csatzo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Feedback
- Survey Tools
- Free Worksheets
- Product Development
- Marketing
---
