---
anonymous_access: false
api_key_in: []
api_specs:
- filename: businessvaluationcost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Business Valuation Cost Enquiry API
  slug: businessvaluationcost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessvaluationcost-co-uk/openapi/businessvaluationcost-co-uk-enquiry-api-openapi.yml
- filename: businessvaluationcost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Business Valuation Cost MCP API
  slug: businessvaluationcost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessvaluationcost-co-uk/openapi/businessvaluationcost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Business Valuation Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Business Valuation Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Business Valuation Cost
provider_slug: businessvaluationcost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/businessvaluationcost-co-uk-openapi.json
  type: http
slug: businessvaluationcost-co-uk-authentication
source_filename: businessvaluationcost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/businessvaluationcost-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/businessvaluationcost-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/businessvaluationcost-co-uk/authentication/businessvaluationcost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Business Valuation
- United Kingdom
- Finance
- Guidance
- Valuation
---
