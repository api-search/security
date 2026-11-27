---
anonymous_access: false
api_key_in: []
api_specs:
- filename: floridaroofreplacementcost-com-enquiry-api-openapi.yml
  format: yaml
  label: floridaroofreplacementcost-com Enquiry API
  slug: floridaroofreplacementcost-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/floridaroofreplacementcost-com/openapi/floridaroofreplacementcost-com-enquiry-api-openapi.yml
- filename: floridaroofreplacementcost-com-mcp-api-openapi.yml
  format: yaml
  label: floridaroofreplacementcost-com MCP API
  slug: floridaroofreplacementcost-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/floridaroofreplacementcost-com/openapi/floridaroofreplacementcost-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: floridaroofreplacementcost-com Authentication
name_suffix: Authentication
oauth_flows: []
overview: floridaroofreplacementcost-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: floridaroofreplacementcost-com
provider_slug: floridaroofreplacementcost-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/floridaroofreplacementcost-com-openapi.json
  type: http
slug: floridaroofreplacementcost-com-authentication
source_filename: floridaroofreplacementcost-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/floridaroofreplacementcost-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/floridaroofreplacementcost-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/floridaroofreplacementcost-com/authentication/floridaroofreplacementcost-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Roofing
- Homeowners
- Insurance
- Building Code
---
