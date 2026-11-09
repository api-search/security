---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dsearassessmentcost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: DSEAR Assessment Cost Enquiry API
  slug: dsearassessmentcost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dsearassessmentcost-co-uk/openapi/dsearassessmentcost-co-uk-enquiry-api-openapi.yml
- filename: dsearassessmentcost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: DSEAR Assessment Cost MCP API
  slug: dsearassessmentcost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dsearassessmentcost-co-uk/openapi/dsearassessmentcost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Dsearassessmentcost Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: DSEAR Assessment Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DSEAR Assessment Cost
provider_slug: dsearassessmentcost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/dsearassessmentcost-co-uk-openapi.json
  type: http
slug: dsearassessmentcost-co-uk-authentication
source_filename: dsearassessmentcost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/dsearassessmentcost-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/dsearassessmentcost-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/dsearassessmentcost-co-uk/authentication/dsearassessmentcost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Risk Assessment
- hazardous area classification
- workplace health and safety
- DSEAR consultancy
---
