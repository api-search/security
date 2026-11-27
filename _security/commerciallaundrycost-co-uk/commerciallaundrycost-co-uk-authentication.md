---
anonymous_access: false
api_key_in: []
api_specs:
- filename: commerciallaundrycost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Commercial Laundry Cost Enquiry API
  slug: commerciallaundrycost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commerciallaundrycost-co-uk/openapi/commerciallaundrycost-co-uk-enquiry-api-openapi.yml
- filename: commerciallaundrycost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Commercial Laundry Cost MCP API
  slug: commerciallaundrycost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commerciallaundrycost-co-uk/openapi/commerciallaundrycost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Commercial Laundry Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Commercial Laundry Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Commercial Laundry Cost
provider_slug: commerciallaundrycost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  optional: true
  scheme: bearer
  sources:
  - openapi/commerciallaundrycost-co-uk-openapi.yml
  - https://commerciallaundrycost.co.uk/openapi.json
  type: http
slug: commerciallaundrycost-co-uk-authentication
source_filename: commerciallaundrycost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commerciallaundrycost.co.uk/openapi.json\ndocs: https://commerciallaundrycost.co.uk/mcp\nsummary:\n  types:\n  - http\n  required: false\n  note: 'Every operation declares security [{}, {accessKey: []}], i.e. anonymous calls are allowed and the\n    bearer access key is optional. The provider-served MCP card (GET /mcp) states \"auth\": \"none\" for the MCP endpoint.\n    No documentation describes how an access key is obtained.'\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  optional: true\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/commerciallaundrycost-co-uk-openapi.yml\n  - https://commerciallaundrycost.co.uk/openapi.json\n"
source_yaml_url: https://artifacts.apis.io/commerciallaundrycost-co-uk/authentication/commerciallaundrycost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Commercial Laundry
- Laundry Equipment
- Cost Guides
- Lead Generation
- Quotes
- United Kingdom
- MCP
---
