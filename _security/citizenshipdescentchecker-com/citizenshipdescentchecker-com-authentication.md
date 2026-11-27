---
anonymous_access: false
api_key_in: []
api_specs:
- filename: citizenshipdescentchecker-com-enquiry-api-openapi.yml
  format: yaml
  label: Citizenship Descent Checker Enquiry API
  slug: citizenshipdescentchecker-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citizenshipdescentchecker-com/openapi/citizenshipdescentchecker-com-enquiry-api-openapi.yml
- filename: citizenshipdescentchecker-com-guide-api-openapi.yml
  format: yaml
  label: Citizenship Descent Checker Guide API
  slug: citizenshipdescentchecker-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citizenshipdescentchecker-com/openapi/citizenshipdescentchecker-com-guide-api-openapi.yml
- filename: citizenshipdescentchecker-com-mcp-api-openapi.yml
  format: yaml
  label: Citizenship Descent Checker MCP API
  slug: citizenshipdescentchecker-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citizenshipdescentchecker-com/openapi/citizenshipdescentchecker-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Citizenship Descent Checker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Citizenship Descent Checker secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Citizenship Descent Checker
provider_slug: citizenshipdescentchecker-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/citizenshipdescentchecker-com-openapi.json
  - openapi/openapi.json
  type: http
slug: citizenshipdescentchecker-com-authentication
source_filename: citizenshipdescentchecker-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/citizenshipdescentchecker-com-openapi.json, openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/citizenshipdescentchecker-com-openapi.json\n  - openapi/openapi.json\n"
source_yaml_url: https://artifacts.apis.io/citizenshipdescentchecker-com/authentication/citizenshipdescentchecker-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Citizenship
- Descent
- Canada
- Immigration
- Guides
---
