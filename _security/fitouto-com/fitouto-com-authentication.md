---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fitouto-com-dataset-api-openapi.yml
  format: yaml
  label: Fitouto Dataset API
  slug: fitouto-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fitouto-com/openapi/fitouto-com-dataset-api-openapi.yml
- filename: fitouto-com-mcp-api-openapi.yml
  format: yaml
  label: Fitouto MCP API
  slug: fitouto-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fitouto-com/openapi/fitouto-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fitouto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fitouto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fitouto
provider_slug: fitouto-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/fitouto-com-openapi.yml
  type: http
slug: fitouto-com-authentication
source_filename: fitouto-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/fitouto-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/fitouto-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/fitouto-com/authentication/fitouto-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Office
- Management
- Software-as-a-Service
- Paperless
- Small Business
---
