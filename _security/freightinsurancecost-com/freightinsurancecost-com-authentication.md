---
anonymous_access: false
api_key_in: []
api_specs:
- filename: freightinsurancecost-com-enquiry-api-openapi.yml
  format: yaml
  label: freightinsurancecost-com Enquiry API
  slug: freightinsurancecost-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freightinsurancecost-com/openapi/freightinsurancecost-com-enquiry-api-openapi.yml
- filename: freightinsurancecost-com-mcp-api-openapi.yml
  format: yaml
  label: freightinsurancecost-com MCP API
  slug: freightinsurancecost-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freightinsurancecost-com/openapi/freightinsurancecost-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: freightinsurancecost-com Authentication
name_suffix: Authentication
oauth_flows: []
overview: freightinsurancecost-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: freightinsurancecost-com
provider_slug: freightinsurancecost-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/freightinsurancecost-com-openapi.json
  type: http
slug: freightinsurancecost-com-authentication
source_filename: freightinsurancecost-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/freightinsurancecost-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/freightinsurancecost-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/freightinsurancecost-com/authentication/freightinsurancecost-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Marine cargo insurance
- Freight Forwarding
- Insurance information
---
