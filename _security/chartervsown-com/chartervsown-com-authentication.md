---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chartervsown-com-calculator-api-openapi.yml
  format: yaml
  label: Charter vs Own Calculator API
  slug: chartervsown-com-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartervsown-com/openapi/chartervsown-com-calculator-api-openapi.yml
- filename: chartervsown-com-enquiry-api-openapi.yml
  format: yaml
  label: Charter vs Own Enquiry API
  slug: chartervsown-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartervsown-com/openapi/chartervsown-com-enquiry-api-openapi.yml
- filename: chartervsown-com-mcp-api-openapi.yml
  format: yaml
  label: Charter vs Own MCP API
  slug: chartervsown-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartervsown-com/openapi/chartervsown-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Chartervsown Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Charter vs Own secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Charter vs Own
provider_slug: chartervsown-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/chartervsown-com-openapi.json
  type: http
slug: chartervsown-com-authentication
source_filename: chartervsown-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/chartervsown-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/chartervsown-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/chartervsown-com/authentication/chartervsown-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Aviation
- Finance
- Calculator
- Private-Jet
- CostEstimator
---
