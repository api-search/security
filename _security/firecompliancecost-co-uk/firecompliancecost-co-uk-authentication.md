---
anonymous_access: false
api_key_in: []
api_specs:
- filename: firecompliancecost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Fire Compliance Cost Enquiry API
  slug: firecompliancecost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firecompliancecost-co-uk/openapi/firecompliancecost-co-uk-enquiry-api-openapi.yml
- filename: firecompliancecost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Fire Compliance Cost MCP API
  slug: firecompliancecost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firecompliancecost-co-uk/openapi/firecompliancecost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Firecompliancecost Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fire Compliance Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fire Compliance Cost
provider_slug: firecompliancecost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/firecompliancecost-co-uk-openapi.json
  type: http
slug: firecompliancecost-co-uk-authentication
source_filename: firecompliancecost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/firecompliancecost-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/firecompliancecost-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/firecompliancecost-co-uk/authentication/firecompliancecost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Fire Safety
- Compliance
- Cost Estimation
- UK
- Free Quotes
---
