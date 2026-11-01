---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clientvo-com-dataset-api-openapi.yml
  format: yaml
  label: clientvo-com Dataset API
  slug: clientvo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clientvo-com/openapi/clientvo-com-dataset-api-openapi.yml
- filename: clientvo-com-mcp-api-openapi.yml
  format: yaml
  label: clientvo-com MCP API
  slug: clientvo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clientvo-com/openapi/clientvo-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Clientvo Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: clientvo-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: clientvo-com
provider_slug: clientvo-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/app-clientvo-openapi.json
  - openapi/clientvo-com-openapi.json
  type: http
slug: clientvo-com-authentication
source_filename: clientvo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/app-clientvo-openapi.json, openapi/clientvo-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/app-clientvo-openapi.json\n  - openapi/clientvo-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/clientvo-com/authentication/clientvo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Payments
- Lending
- Compliance
- KYC
---
