---
api_key_in: []
api_specs:
- filename: quadratic-openapi.json
  format: json
  label: Quadratic Developer API
  slug: quadratic-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/openapi/quadratic-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Quadratic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quadratic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Quadratic
provider_slug: quadratic
scheme_count: 1
schemes:
- bearerFormat: API token (qdx_live_… or qdx_test_…)
  description: 'API tokens are minted from the Quadratic UI under Team Settings → API Tokens. Send as `Authorization: Bearer <token>`.'
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/quadratic-openapi.json
  type: http
slug: quadratic-authentication
source_filename: quadratic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/quadratic-openapi.json; https://www.quadratichq.com/spreadsheet-api\ndocs: https://www.quadratichq.com/spreadsheet-api\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  bearerFormat: API token (qdx_live_… or qdx_test_…)\n  description: 'API tokens are minted from the Quadratic UI under Team Settings → API Tokens.\n    Send as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/quadratic-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/authentication/quadratic-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Spreadsheet
- Analytics
- Data
- Developer Tools
- MCP
- Productivity
---
