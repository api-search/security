---
anonymous_access: false
api_key_in: []
api_specs:
- filename: forsaccreditationcost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: FORS Accreditation Cost Enquiry API
  slug: forsaccreditationcost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forsaccreditationcost-co-uk/openapi/forsaccreditationcost-co-uk-enquiry-api-openapi.yml
- filename: forsaccreditationcost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: FORS Accreditation Cost MCP API
  slug: forsaccreditationcost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forsaccreditationcost-co-uk/openapi/forsaccreditationcost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: FORS Accreditation Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: FORS Accreditation Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FORS Accreditation Cost
provider_slug: forsaccreditationcost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/forsaccreditationcost-co-uk-openapi.json
  type: http
slug: forsaccreditationcost-co-uk-authentication
source_filename: forsaccreditationcost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/forsaccreditationcost-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/forsaccreditationcost-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/forsaccreditationcost-co-uk/authentication/forsaccreditationcost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Transportation
- Accreditation
- United Kingdom
- Fees
- Compliance
- Company
---
