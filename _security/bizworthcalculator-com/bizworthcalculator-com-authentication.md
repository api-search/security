---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bizworthcalculator-com-calculator-api-openapi.yml
  format: yaml
  label: Value My Business Calculator Calculator API
  slug: bizworthcalculator-com-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bizworthcalculator-com/openapi/bizworthcalculator-com-calculator-api-openapi.yml
- filename: bizworthcalculator-com-enquiry-api-openapi.yml
  format: yaml
  label: Value My Business Calculator Enquiry API
  slug: bizworthcalculator-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bizworthcalculator-com/openapi/bizworthcalculator-com-enquiry-api-openapi.yml
- filename: bizworthcalculator-com-mcp-api-openapi.yml
  format: yaml
  label: Value My Business Calculator MCP API
  slug: bizworthcalculator-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bizworthcalculator-com/openapi/bizworthcalculator-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bizworthcalculator Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Value My Business Calculator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Value My Business Calculator
provider_slug: bizworthcalculator-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/bizworthcalculator-com-openapi.json
  type: http
slug: bizworthcalculator-com-authentication
source_filename: bizworthcalculator-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/bizworthcalculator-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/bizworthcalculator-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/bizworthcalculator-com/authentication/bizworthcalculator-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Business
- Valuation
- Calculator
- Small Business
- Finance
---
