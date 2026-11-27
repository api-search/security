---
anonymous_access: false
api_key_in: []
api_specs:
- filename: deflectvo-com-dataset-api-openapi.yml
  format: yaml
  label: Deflectvo Dataset API
  slug: deflectvo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deflectvo-com/openapi/deflectvo-com-dataset-api-openapi.yml
- filename: deflectvo-com-mcp-api-openapi.yml
  format: yaml
  label: Deflectvo MCP API
  slug: deflectvo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deflectvo-com/openapi/deflectvo-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Deflectvo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deflectvo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Deflectvo
provider_slug: deflectvo-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/deflectvo-com-openapi.yml
  type: http
slug: deflectvo-com-authentication
source_filename: deflectvo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/deflectvo-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/deflectvo-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/deflectvo-com/authentication/deflectvo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Customer Self-Service
- Customer Service
- Help Center
- Ticket Deflection
- Customer Portal
- Software-as-a-Service
---
