---
anonymous_access: false
api_key_in: []
api_specs:
- filename: disclovo-com-dataset-api-openapi.yml
  format: yaml
  label: Disclovo Dataset API
  slug: disclovo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disclovo-com/openapi/disclovo-com-dataset-api-openapi.yml
- filename: disclovo-com-mcp-api-openapi.yml
  format: yaml
  label: Disclovo MCP API
  slug: disclovo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disclovo-com/openapi/disclovo-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Disclovo Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Disclovo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Disclovo
provider_slug: disclovo-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/disclovo-com-openapi.yml
  type: http
slug: disclovo-com-authentication
source_filename: disclovo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/disclovo-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/disclovo-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/disclovo-com/authentication/disclovo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Regulatory
- Reporting
- Compliance
- Software
- Finance
---
