---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dataroompicker-com-enquiry-api-openapi.yml
  format: yaml
  label: Data Room Picker Enquiry API
  slug: dataroompicker-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataroompicker-com/openapi/dataroompicker-com-enquiry-api-openapi.yml
- filename: dataroompicker-com-guide-api-openapi.yml
  format: yaml
  label: Data Room Picker Guide API
  slug: dataroompicker-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataroompicker-com/openapi/dataroompicker-com-guide-api-openapi.yml
- filename: dataroompicker-com-mcp-api-openapi.yml
  format: yaml
  label: Data Room Picker MCP API
  slug: dataroompicker-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataroompicker-com/openapi/dataroompicker-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Data Room Picker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Data Room Picker secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Data Room Picker
provider_slug: dataroompicker-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/dataroompicker-com-openapi.json
  type: http
slug: dataroompicker-com-authentication
source_filename: dataroompicker-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/dataroompicker-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/dataroompicker-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/dataroompicker-com/authentication/dataroompicker-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Data
- Pricing
- Virtual Data Room
- Comparison
- M&A
---
