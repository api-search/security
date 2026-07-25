---
api_key_in: []
api_specs:
- filename: quadratic-agent-connections-api-openapi.yml
  format: yaml
  label: Quadratic Agent Connections API
  slug: quadratic-agent-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/openapi/quadratic-agent-connections-api-openapi.yml
- filename: quadratic-auth-api-openapi.yml
  format: yaml
  label: Quadratic Auth API
  slug: quadratic-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/openapi/quadratic-auth-api-openapi.yml
- filename: quadratic-cells-api-openapi.yml
  format: yaml
  label: Quadratic Cells API
  slug: quadratic-cells-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/openapi/quadratic-cells-api-openapi.yml
- filename: quadratic-columns-and-rows-api-openapi.yml
  format: yaml
  label: Quadratic Columns and rows API
  slug: quadratic-columns-and-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/openapi/quadratic-columns-and-rows-api-openapi.yml
- filename: quadratic-conditional-formats-api-openapi.yml
  format: yaml
  label: Quadratic Conditional formats API
  slug: quadratic-conditional-formats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/openapi/quadratic-conditional-formats-api-openapi.yml
- filename: quadratic-connections-api-openapi.yml
  format: yaml
  label: Quadratic Connections API
  slug: quadratic-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/openapi/quadratic-connections-api-openapi.yml
- filename: quadratic-context-outline-search-api-openapi.yml
  format: yaml
  label: Quadratic Context, outline, search API
  slug: quadratic-context-outline-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/openapi/quadratic-context-outline-search-api-openapi.yml
- filename: quadratic-documentation-api-openapi.yml
  format: yaml
  label: Quadratic Documentation API
  slug: quadratic-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/openapi/quadratic-documentation-api-openapi.yml
- filename: quadratic-files-api-openapi.yml
  format: yaml
  label: Quadratic Files API
  slug: quadratic-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/openapi/quadratic-files-api-openapi.yml
- filename: quadratic-health-api-openapi.yml
  format: yaml
  label: Quadratic Health API
  slug: quadratic-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/openapi/quadratic-health-api-openapi.yml
- filename: quadratic-history-api-openapi.yml
  format: yaml
  label: Quadratic History API
  slug: quadratic-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/openapi/quadratic-history-api-openapi.yml
- filename: quadratic-sheets-api-openapi.yml
  format: yaml
  label: Quadratic Sheets API
  slug: quadratic-sheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/openapi/quadratic-sheets-api-openapi.yml
- filename: quadratic-tables-api-openapi.yml
  format: yaml
  label: Quadratic Tables API
  slug: quadratic-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/openapi/quadratic-tables-api-openapi.yml
- filename: quadratic-validations-api-openapi.yml
  format: yaml
  label: Quadratic Validations API
  slug: quadratic-validations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/openapi/quadratic-validations-api-openapi.yml
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
