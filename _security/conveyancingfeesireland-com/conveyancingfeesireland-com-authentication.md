---
anonymous_access: false
api_key_in: []
api_specs:
- filename: conveyancingfeesireland-com-enquiry-api-openapi.yml
  format: yaml
  label: Conveyancing Fees Ireland Enquiry API
  slug: conveyancingfeesireland-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conveyancingfeesireland-com/openapi/conveyancingfeesireland-com-enquiry-api-openapi.yml
- filename: conveyancingfeesireland-com-mcp-api-openapi.yml
  format: yaml
  label: Conveyancing Fees Ireland MCP API
  slug: conveyancingfeesireland-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conveyancingfeesireland-com/openapi/conveyancingfeesireland-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Conveyancing Fees Ireland Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conveyancing Fees Ireland secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Conveyancing Fees Ireland
provider_slug: conveyancingfeesireland-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/conveyancingfeesireland-com-openapi.yml
  type: http
slug: conveyancingfeesireland-com-authentication
source_filename: conveyancingfeesireland-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/conveyancingfeesireland-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/conveyancingfeesireland-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/conveyancingfeesireland-com/authentication/conveyancingfeesireland-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Conveyancing
- Legal Services
- Real Estate
- Ireland
- Stamp Duty
- Property
- Open Data
---
