---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cctvinstallationcost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: CCTV Installation Cost Enquiry API
  slug: cctvinstallationcost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cctvinstallationcost-co-uk/openapi/cctvinstallationcost-co-uk-enquiry-api-openapi.yml
- filename: cctvinstallationcost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: CCTV Installation Cost MCP API
  slug: cctvinstallationcost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cctvinstallationcost-co-uk/openapi/cctvinstallationcost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cctvinstallationcost Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: CCTV Installation Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CCTV Installation Cost
provider_slug: cctvinstallationcost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/cctvinstallationcost-co-uk-openapi.json
  type: http
slug: cctvinstallationcost-co-uk-authentication
source_filename: cctvinstallationcost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/cctvinstallationcost-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/cctvinstallationcost-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cctvinstallationcost-co-uk/authentication/cctvinstallationcost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- CCTV
- Installations
- Quotes
- United Kingdom
---
