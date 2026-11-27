---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getgenko-com-analytics-api-openapi.yml
  format: yaml
  label: Genkō Analytics API
  slug: getgenko-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getgenko-com/openapi/getgenko-com-analytics-api-openapi.yml
- filename: getgenko-com-mcp-api-openapi.yml
  format: yaml
  label: Genkō MCP API
  slug: getgenko-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getgenko-com/openapi/getgenko-com-mcp-api-openapi.yml
- filename: getgenko-com-risk-api-openapi.yml
  format: yaml
  label: Genkō Risk API
  slug: getgenko-com-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getgenko-com/openapi/getgenko-com-risk-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Genkō Authentication
name_suffix: Authentication
oauth_flows: []
overview: Genkō secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Genkō
provider_slug: getgenko-com
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: 'Generate an API key from an invited private-beta account in Dashboard → Settings → API Keys. Pass as: Authorization: Bearer gk_<key>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/getgenko-com-openapi.json
  type: http
slug: getgenko-com-authentication
source_filename: getgenko-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/getgenko-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: 'Generate an API key from an invited private-beta account in Dashboard → Settings\n    → API Keys. Pass as: Authorization: Bearer gk_<key>'\n  sources:\n  - openapi/getgenko-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/getgenko-com/authentication/getgenko-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- Scheduling
- Electronic Health Records
- Software-as-a-Service
- Clinics
---
