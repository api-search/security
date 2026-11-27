---
anonymous_access: false
api_key_in: []
api_specs:
- filename: basementexcavationcost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Basement Excavation Cost Enquiry API
  slug: basementexcavationcost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basementexcavationcost-co-uk/openapi/basementexcavationcost-co-uk-enquiry-api-openapi.yml
- filename: basementexcavationcost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Basement Excavation Cost MCP API
  slug: basementexcavationcost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basementexcavationcost-co-uk/openapi/basementexcavationcost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Basement Excavation Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Basement Excavation Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Basement Excavation Cost
provider_slug: basementexcavationcost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/basementexcavationcost-co-uk-openapi.json
  - openapi/openapi.json
  type: http
slug: basementexcavationcost-co-uk-authentication
source_filename: basementexcavationcost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/basementexcavationcost-co-uk-openapi.json, openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/basementexcavationcost-co-uk-openapi.json\n  - openapi/openapi.json\n"
source_yaml_url: https://artifacts.apis.io/basementexcavationcost-co-uk/authentication/basementexcavationcost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Construction
- Real Estate
- Cost Estimation
- United Kingdom
---
