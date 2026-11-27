---
anonymous_access: false
api_key_in: []
api_specs:
- filename: focusvo-com-dataset-api-openapi.yml
  format: yaml
  label: Focusvo Dataset API
  slug: focusvo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/focusvo-com/openapi/focusvo-com-dataset-api-openapi.yml
- filename: focusvo-com-mcp-api-openapi.yml
  format: yaml
  label: Focusvo MCP API
  slug: focusvo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/focusvo-com/openapi/focusvo-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Focusvo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Focusvo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Focusvo
provider_slug: focusvo-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/focusvo-com-openapi.json
  type: http
slug: focusvo-com-authentication
source_filename: focusvo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/focusvo-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/focusvo-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/focusvo-com/authentication/focusvo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Accessibility
- Compliance
- Tools
- ADA
- US Business
---
