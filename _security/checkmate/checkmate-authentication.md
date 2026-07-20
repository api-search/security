---
api_key_in:
- header
api_specs:
- filename: checkmate-openstock-openapi-original.json
  format: json
  label: OpenStock API
  slug: openstock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmate/refs/heads/main/openapi/checkmate-openstock-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Checkmate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Checkmate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Checkmate
provider_slug: checkmate
scheme_count: 1
schemes:
- description: Partner API key issued by a Checkmate/OpenStock partner representative ("Ask partner representative for the API key"). Presented as an HTTP bearer token on every request except GET /health. Missing or invalid keys return 401. Rate limits are enforced per partner.
  format: 'Authorization: Bearer <api_key>'
  in: header
  name: bearerApiKey
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/checkmate-openstock-openapi-original.json
  type: http
slug: checkmate-authentication
source_filename: checkmate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.openstock.sh/openapi.json (info.description) + https://openstock.sh\ndocs: https://api.openstock.sh/docs\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    The OpenStock OpenAPI does not declare a formal components.securitySchemes\n    block; authentication is documented in prose in the spec description and on\n    the OpenStock site. All authenticated endpoints require a bearer API key.\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Bearer <api_key>'\n  description: >-\n    Partner API key issued by a Checkmate/OpenStock partner representative\n    (\"Ask partner representative for the API key\"). Presented as an\n    HTTP bearer token on every request except GET /health. Missing or invalid\n    keys return 401. Rate limits are enforced per partner.\n  sources:\n  - openapi/checkmate-openstock-openapi-original.json\n\
  mcp_auth:\n  server: https://mcp.joincheckmate.com\n  scheme: bearer\n  header: Authorization\n  format: 'Authorization: Bearer ${KEY}'\n  note: >-\n    The OpenStock MCP server uses the same bearer credential; a single\n    credential grants access to the entire 284,000+ merchant network.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkmate/refs/heads/main/authentication/checkmate-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- Commerce
- Ecommerce
- Shopping
- Discount Codes
- Coupons
- Merchants
- MCP
- Agentic Commerce
- Retail
- API
---
