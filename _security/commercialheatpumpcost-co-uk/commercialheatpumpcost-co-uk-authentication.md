---
anonymous_access: true
api_key_in: []
api_specs:
- filename: commercialheatpumpcost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Commercial Heat Pump Cost Enquiry API
  slug: commercialheatpumpcost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commercialheatpumpcost-co-uk/openapi/commercialheatpumpcost-co-uk-enquiry-api-openapi.yml
- filename: commercialheatpumpcost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Commercial Heat Pump Cost MCP API
  slug: commercialheatpumpcost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commercialheatpumpcost-co-uk/openapi/commercialheatpumpcost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Commercial Heat Pump Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Commercial Heat Pump Cost secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Commercial Heat Pump Cost
provider_slug: commercialheatpumpcost-co-uk
scheme_count: 2
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  required: false
  scheme: bearer
  sources:
  - openapi/commercialheatpumpcost-co-uk-openapi.yml
  type: http
- description: MCP card at https://commercialheatpumpcost.co.uk/mcp declares auth "none", transport streamable-http, stateless.
  name: none
  sources:
  - https://commercialheatpumpcost.co.uk/mcp
  type: none
slug: commercialheatpumpcost-co-uk-authentication
source_filename: commercialheatpumpcost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commercialheatpumpcost.co.uk/mcp\ndocs: https://commercialheatpumpcost.co.uk/mcp\nsummary:\n  types:\n  - http\n  anonymous_access: true\n  note: 'The MCP card (GET /mcp, HTTP 200) declares \"auth\": \"none\" for the MCP endpoint. The OpenAPI declares an optional bearer access key (emk_...) that lifts the free-tier ceiling. No document was found that explains how to get a key. The 429 response points to \"docs/MCP.md\", but https://commercialheatpumpcost.co.uk/docs/MCP.md returned HTTP 404 on 2026-11-04.'\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  required: false\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/commercialheatpumpcost-co-uk-openapi.yml\n- name: none\n  type: none\n  description: MCP card at https://commercialheatpumpcost.co.uk/mcp declares auth \"none\", transport streamable-http,\
  \ stateless.\n  sources:\n  - https://commercialheatpumpcost.co.uk/mcp\n"
source_yaml_url: https://artifacts.apis.io/commercialheatpumpcost-co-uk/authentication/commercialheatpumpcost-co-uk-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Heat Pumps
- Renewable Energy
- Commercial Heating
- Energy Prices
- Open Data
- United Kingdom
- Grants
---
