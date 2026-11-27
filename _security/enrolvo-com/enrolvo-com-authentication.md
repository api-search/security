---
anonymous_access: false
api_key_in: []
api_specs:
- filename: enrolvo-com-dataset-api-openapi.yml
  format: yaml
  label: Enrolvo Dataset API
  slug: enrolvo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enrolvo-com/openapi/enrolvo-com-dataset-api-openapi.yml
- filename: enrolvo-com-mcp-api-openapi.yml
  format: yaml
  label: Enrolvo MCP API
  slug: enrolvo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enrolvo-com/openapi/enrolvo-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Enrolvo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enrolvo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Enrolvo
provider_slug: enrolvo-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/enrolvo-com-openapi.json
  type: http
slug: enrolvo-com-authentication
source_filename: enrolvo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/enrolvo-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/enrolvo-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/enrolvo-com/authentication/enrolvo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Continuing Education
- Education Accounting
- Payroll
- Certificate Management
- Small Provider Software
---
