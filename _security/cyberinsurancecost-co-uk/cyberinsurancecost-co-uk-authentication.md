---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cyberinsurancecost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Cyber Insurance Cost Enquiry API
  slug: cyberinsurancecost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberinsurancecost-co-uk/openapi/cyberinsurancecost-co-uk-enquiry-api-openapi.yml
- filename: cyberinsurancecost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Cyber Insurance Cost MCP API
  slug: cyberinsurancecost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberinsurancecost-co-uk/openapi/cyberinsurancecost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cyberinsurancecost Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cyber Insurance Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cyber Insurance Cost
provider_slug: cyberinsurancecost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/cyberinsurancecost-co-uk-openapi.json
  type: http
slug: cyberinsurancecost-co-uk-authentication
source_filename: cyberinsurancecost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/cyberinsurancecost-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/cyberinsurancecost-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cyberinsurancecost-co-uk/authentication/cyberinsurancecost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Cyber Insurance
- UK Small Business
- Insurance
- Risk Management
- Data
- Pricing
---
