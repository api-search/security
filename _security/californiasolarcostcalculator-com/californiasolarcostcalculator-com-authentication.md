---
anonymous_access: false
api_key_in: []
api_specs:
- filename: californiasolarcostcalculator-com-calculator-api-openapi.yml
  format: yaml
  label: California Solar Cost Calculator Calculator API
  slug: californiasolarcostcalculator-com-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/californiasolarcostcalculator-com/openapi/californiasolarcostcalculator-com-calculator-api-openapi.yml
- filename: californiasolarcostcalculator-com-enquiry-api-openapi.yml
  format: yaml
  label: California Solar Cost Calculator Enquiry API
  slug: californiasolarcostcalculator-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/californiasolarcostcalculator-com/openapi/californiasolarcostcalculator-com-enquiry-api-openapi.yml
- filename: californiasolarcostcalculator-com-mcp-api-openapi.yml
  format: yaml
  label: California Solar Cost Calculator MCP API
  slug: californiasolarcostcalculator-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/californiasolarcostcalculator-com/openapi/californiasolarcostcalculator-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Californiasolarcostcalculator Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: California Solar Cost Calculator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: California Solar Cost Calculator
provider_slug: californiasolarcostcalculator-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/californiasolarcostcalculator-com-openapi.json
  - openapi/openapi.json
  type: http
slug: californiasolarcostcalculator-com-authentication
source_filename: californiasolarcostcalculator-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/californiasolarcostcalculator-com-openapi.json, openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/californiasolarcostcalculator-com-openapi.json\n  - openapi/openapi.json\n"
source_yaml_url: https://artifacts.apis.io/californiasolarcostcalculator-com/authentication/californiasolarcostcalculator-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Solar
- Calculator
- California
- Energy
- Finance
- Company
---
