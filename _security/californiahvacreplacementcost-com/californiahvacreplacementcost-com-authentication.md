---
anonymous_access: false
api_key_in: []
api_specs:
- filename: californiahvacreplacementcost-com-enquiry-api-openapi.yml
  format: yaml
  label: California HVAC Replacement Cost Enquiry API
  slug: californiahvacreplacementcost-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/californiahvacreplacementcost-com/openapi/californiahvacreplacementcost-com-enquiry-api-openapi.yml
- filename: californiahvacreplacementcost-com-mcp-api-openapi.yml
  format: yaml
  label: California HVAC Replacement Cost MCP API
  slug: californiahvacreplacementcost-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/californiahvacreplacementcost-com/openapi/californiahvacreplacementcost-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Californiahvacreplacementcost Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: California HVAC Replacement Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: California HVAC Replacement Cost
provider_slug: californiahvacreplacementcost-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/californiahvacreplacementcost-com-openapi.json
  type: http
slug: californiahvacreplacementcost-com-authentication
source_filename: californiahvacreplacementcost-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/californiahvacreplacementcost-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/californiahvacreplacementcost-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/californiahvacreplacementcost-com/authentication/californiahvacreplacementcost-com-authentication.yml
summary_line: http · 1 scheme
tags:
- HVAC
- California
- Replacement
- Cost
- Energy
---
