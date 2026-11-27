---
anonymous_access: false
api_key_in: []
api_specs:
- filename: conveyancingfees-co-nz-enquiry-api-openapi.yml
  format: yaml
  label: Conveyancing Fees NZ Enquiry API
  slug: conveyancingfees-co-nz-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conveyancingfees-co-nz/openapi/conveyancingfees-co-nz-enquiry-api-openapi.yml
- filename: conveyancingfees-co-nz-mcp-api-openapi.yml
  format: yaml
  label: Conveyancing Fees NZ MCP API
  slug: conveyancingfees-co-nz-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conveyancingfees-co-nz/openapi/conveyancingfees-co-nz-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Conveyancing Fees NZ Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conveyancing Fees NZ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Conveyancing Fees NZ
provider_slug: conveyancingfees-co-nz
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/conveyancingfees-co-nz-openapi.yml
  type: http
slug: conveyancingfees-co-nz-authentication
source_filename: conveyancingfees-co-nz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/conveyancingfees-co-nz-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/conveyancingfees-co-nz-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/conveyancingfees-co-nz/authentication/conveyancingfees-co-nz-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Conveyancing
- Real Estate
- Legal Services
- Property
- New Zealand
- Datasets
- Quotes
---
