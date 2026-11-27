---
anonymous_access: false
api_key_in: []
api_specs:
- filename: executivesearchfees-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Executive Search Fees Enquiry API
  slug: executivesearchfees-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/executivesearchfees-co-uk/openapi/executivesearchfees-co-uk-enquiry-api-openapi.yml
- filename: executivesearchfees-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Executive Search Fees MCP API
  slug: executivesearchfees-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/executivesearchfees-co-uk/openapi/executivesearchfees-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Executive Search Fees Authentication
name_suffix: Authentication
oauth_flows: []
overview: Executive Search Fees secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Executive Search Fees
provider_slug: executivesearchfees-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/executivesearchfees-co-uk-openapi.json
  type: http
slug: executivesearchfees-co-uk-authentication
source_filename: executivesearchfees-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/executivesearchfees-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/executivesearchfees-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/executivesearchfees-co-uk/authentication/executivesearchfees-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Executive Search
- Recruiting
- Fees
- United Kingdom
- Guidance
---
