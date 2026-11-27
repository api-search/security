---
anonymous_access: false
api_key_in: []
api_specs:
- filename: generatorservicingcost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Generator Servicing Cost Enquiry API
  slug: generatorservicingcost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generatorservicingcost-co-uk/openapi/generatorservicingcost-co-uk-enquiry-api-openapi.yml
- filename: generatorservicingcost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Generator Servicing Cost MCP API
  slug: generatorservicingcost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generatorservicingcost-co-uk/openapi/generatorservicingcost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Generator Servicing Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Generator Servicing Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Generator Servicing Cost
provider_slug: generatorservicingcost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/generatorservicingcost-co-uk-openapi.json
  type: http
slug: generatorservicingcost-co-uk-authentication
source_filename: generatorservicingcost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/generatorservicingcost-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/generatorservicingcost-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/generatorservicingcost-co-uk/authentication/generatorservicingcost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Energy
- Maintenance
- United Kingdom
- Generators
---
