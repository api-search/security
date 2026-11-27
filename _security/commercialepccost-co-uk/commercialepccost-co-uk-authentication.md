---
anonymous_access: false
api_key_in: []
api_specs:
- filename: commercialepccost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Commercial EPC Cost Enquiry API
  slug: commercialepccost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commercialepccost-co-uk/openapi/commercialepccost-co-uk-enquiry-api-openapi.yml
- filename: commercialepccost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Commercial EPC Cost MCP API
  slug: commercialepccost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commercialepccost-co-uk/openapi/commercialepccost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Commercial EPC Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Commercial EPC Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Commercial EPC Cost
provider_slug: commercialepccost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/commercialepccost-co-uk-openapi.yml
  type: http
slug: commercialepccost-co-uk-authentication
source_filename: commercialepccost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/commercialepccost-co-uk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/commercialepccost-co-uk-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/commercialepccost-co-uk/authentication/commercialepccost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Energy Performance Certificates
- MEES
- Commercial Property
- Energy Efficiency
- United Kingdom
---
