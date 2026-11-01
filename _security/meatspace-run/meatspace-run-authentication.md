---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: meatspace-run-keys-api-openapi.yml
  format: yaml
  label: meatspace-run Keys API
  slug: meatspace-run-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meatspace-run/openapi/meatspace-run-keys-api-openapi.yml
- filename: meatspace-run-mcp-api-openapi.yml
  format: yaml
  label: meatspace-run MCP API
  slug: meatspace-run-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meatspace-run/openapi/meatspace-run-mcp-api-openapi.yml
- filename: meatspace-run-requests-api-openapi.yml
  format: yaml
  label: meatspace-run Requests API
  slug: meatspace-run-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meatspace-run/openapi/meatspace-run-requests-api-openapi.yml
- filename: meatspace-run-review-api-openapi.yml
  format: yaml
  label: meatspace-run Review API
  slug: meatspace-run-review-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meatspace-run/openapi/meatspace-run-review-api-openapi.yml
- filename: meatspace-run-status-api-openapi.yml
  format: yaml
  label: meatspace-run Status API
  slug: meatspace-run-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meatspace-run/openapi/meatspace-run-status-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Meatspace Run Authentication
name_suffix: Authentication
oauth_flows: []
overview: meatspace-run secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: meatspace-run
provider_slug: meatspace-run
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/meatspace-run-openapi.json
  type: http
- in: cookie
  name: adminSession
  parameter: hitl_admin_session
  sources:
  - openapi/meatspace-run-openapi.json
  type: apiKey
slug: meatspace-run-authentication
source_filename: meatspace-run-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/meatspace-run-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/meatspace-run-openapi.json\n- name: adminSession\n  type: apiKey\n  in: cookie\n  parameter: hitl_admin_session\n  sources:\n  - openapi/meatspace-run-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/meatspace-run/authentication/meatspace-run-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- AI
- Human-in-the-loop
- API
- Automation
---
