---
anonymous_access: false
api_key_in: []
api_specs:
- filename: floridasolarcostcalculator-com-calculator-api-openapi.yml
  format: yaml
  label: Florida Solar Cost Calculator Calculator API
  slug: floridasolarcostcalculator-com-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/floridasolarcostcalculator-com/openapi/floridasolarcostcalculator-com-calculator-api-openapi.yml
- filename: floridasolarcostcalculator-com-enquiry-api-openapi.yml
  format: yaml
  label: Florida Solar Cost Calculator Enquiry API
  slug: floridasolarcostcalculator-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/floridasolarcostcalculator-com/openapi/floridasolarcostcalculator-com-enquiry-api-openapi.yml
- filename: floridasolarcostcalculator-com-mcp-api-openapi.yml
  format: yaml
  label: Florida Solar Cost Calculator MCP API
  slug: floridasolarcostcalculator-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/floridasolarcostcalculator-com/openapi/floridasolarcostcalculator-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Florida Solar Cost Calculator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Florida Solar Cost Calculator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Florida Solar Cost Calculator
provider_slug: floridasolarcostcalculator-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/floridasolarcostcalculator-com-openapi.json
  type: http
slug: floridasolarcostcalculator-com-authentication
source_filename: floridasolarcostcalculator-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/floridasolarcostcalculator-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/floridasolarcostcalculator-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/floridasolarcostcalculator-com/authentication/floridasolarcostcalculator-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Solar
- Calculator
- Florida
- Energy
- Homeowners
---
