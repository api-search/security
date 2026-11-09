---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coldroominstallationcost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Cold Room Installation Cost Enquiry API
  slug: coldroominstallationcost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldroominstallationcost-co-uk/openapi/coldroominstallationcost-co-uk-enquiry-api-openapi.yml
- filename: coldroominstallationcost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Cold Room Installation Cost MCP API
  slug: coldroominstallationcost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldroominstallationcost-co-uk/openapi/coldroominstallationcost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Coldroominstallationcost Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cold Room Installation Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cold Room Installation Cost
provider_slug: coldroominstallationcost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/coldroominstallationcost-co-uk-openapi.json
  type: http
slug: coldroominstallationcost-co-uk-authentication
source_filename: coldroominstallationcost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/coldroominstallationcost-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/coldroominstallationcost-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/coldroominstallationcost-co-uk/authentication/coldroominstallationcost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- ColdRoom
- Installations
- Cost
- United Kingdom
- Refrigeration
- Company
---
