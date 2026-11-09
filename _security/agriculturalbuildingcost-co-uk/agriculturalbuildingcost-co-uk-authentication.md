---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agriculturalbuildingcost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Agricultural Building Cost Enquiry API
  slug: agriculturalbuildingcost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agriculturalbuildingcost-co-uk/openapi/agriculturalbuildingcost-co-uk-enquiry-api-openapi.yml
- filename: agriculturalbuildingcost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Agricultural Building Cost MCP API
  slug: agriculturalbuildingcost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agriculturalbuildingcost-co-uk/openapi/agriculturalbuildingcost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Agriculturalbuildingcost Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agricultural Building Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agricultural Building Cost
provider_slug: agriculturalbuildingcost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/openapi.json
  type: http
slug: agriculturalbuildingcost-co-uk-authentication
source_filename: agriculturalbuildingcost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://artifacts.apis.io/agriculturalbuildingcost-co-uk/authentication/agriculturalbuildingcost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Agriculture
- Construction
- Cost Estimation
- United Kingdom
---
