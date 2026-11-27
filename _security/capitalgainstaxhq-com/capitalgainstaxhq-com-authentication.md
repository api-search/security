---
anonymous_access: false
api_key_in: []
api_specs:
- filename: capitalgainstaxhq-com-dataset-api-openapi.yml
  format: yaml
  label: Capital Gains Tax HQ Dataset API
  slug: capitalgainstaxhq-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capitalgainstaxhq-com/openapi/capitalgainstaxhq-com-dataset-api-openapi.yml
- filename: capitalgainstaxhq-com-enquiry-api-openapi.yml
  format: yaml
  label: Capital Gains Tax HQ Enquiry API
  slug: capitalgainstaxhq-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capitalgainstaxhq-com/openapi/capitalgainstaxhq-com-enquiry-api-openapi.yml
- filename: capitalgainstaxhq-com-mcp-api-openapi.yml
  format: yaml
  label: Capital Gains Tax HQ MCP API
  slug: capitalgainstaxhq-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capitalgainstaxhq-com/openapi/capitalgainstaxhq-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Capital Gains Tax HQ Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capital Gains Tax HQ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Capital Gains Tax HQ
provider_slug: capitalgainstaxhq-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/capitalgainstaxhq-com-openapi.json
  type: http
slug: capitalgainstaxhq-com-authentication
source_filename: capitalgainstaxhq-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/capitalgainstaxhq-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/capitalgainstaxhq-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/capitalgainstaxhq-com/authentication/capitalgainstaxhq-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Tax
- Calculator
- United States
- Capital Gains
---
