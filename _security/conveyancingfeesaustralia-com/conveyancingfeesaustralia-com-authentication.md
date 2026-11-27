---
anonymous_access: false
api_key_in: []
api_specs:
- filename: conveyancingfeesaustralia-com-enquiry-api-openapi.yml
  format: yaml
  label: Conveyancing Fees Australia Enquiry API
  slug: conveyancingfeesaustralia-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conveyancingfeesaustralia-com/openapi/conveyancingfeesaustralia-com-enquiry-api-openapi.yml
- filename: conveyancingfeesaustralia-com-mcp-api-openapi.yml
  format: yaml
  label: Conveyancing Fees Australia MCP API
  slug: conveyancingfeesaustralia-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conveyancingfeesaustralia-com/openapi/conveyancingfeesaustralia-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Conveyancing Fees Australia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conveyancing Fees Australia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Conveyancing Fees Australia
provider_slug: conveyancingfeesaustralia-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/conveyancingfeesaustralia-com-openapi.yml
  type: http
slug: conveyancingfeesaustralia-com-authentication
source_filename: conveyancingfeesaustralia-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/conveyancingfeesaustralia-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/conveyancingfeesaustralia-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/conveyancingfeesaustralia-com/authentication/conveyancingfeesaustralia-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Conveyancing
- Real Estate
- Stamp Duty
- Property
- Australia
- Calculators
- Open Data
---
