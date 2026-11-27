---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cookievo-com-dataset-api-openapi.yml
  format: yaml
  label: Cookievo Dataset API
  slug: cookievo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cookievo-com/openapi/cookievo-com-dataset-api-openapi.yml
- filename: cookievo-com-mcp-api-openapi.yml
  format: yaml
  label: Cookievo MCP API
  slug: cookievo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cookievo-com/openapi/cookievo-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cookievo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cookievo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cookievo
provider_slug: cookievo-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/cookievo-com-openapi.yml
  type: http
slug: cookievo-com-authentication
source_filename: cookievo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/cookievo-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/cookievo-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/cookievo-com/authentication/cookievo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cookie Consent
- Consent Management
- Privacy
- GDPR
- Compliance
- Cookies
---
