---
api_key_in:
- header
api_specs:
- filename: intelligems-external-api-openapi.yml
  format: yaml
  label: Intelligems External API
  slug: intelligems-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/openapi/intelligems-external-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Intelligems Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Intelligems secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Intelligems
provider_slug: intelligems
scheme_count: 2
schemes:
- in: header
  name: accessToken
  notes: Include your Intelligems-issued API key in the `intelligems-access-token` request header. Missing or invalid keys return HTTP 401 with body {"error":"Unauthorized"}.
  parameter_name: intelligems-access-token
  sources:
  - openapi/intelligems-external-api-openapi.yml
  surface: External API (https://api.intelligems.io)
  type: apiKey
- flow: authorizationCode
  name: oauth2
  notes: The hosted Intelligems MCP server is OAuth2-authenticated against an Intelligems organization account; most tools accept an optional `organization` parameter to scope data access.
  sources:
  - mcp/intelligems-mcp.yml
  surface: MCP server (https://ai.intelligems.io/mcp)
  type: oauth2
slug: intelligems-authentication
source_filename: intelligems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.intelligems.io/developer-resources/external-api/intelligems-external-api/authentication\ndocs: https://docs.intelligems.io/developer-resources/external-api/intelligems-external-api/authentication\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: accessToken\n    type: apiKey\n    in: header\n    parameter_name: intelligems-access-token\n    surface: External API (https://api.intelligems.io)\n    notes: >-\n      Include your Intelligems-issued API key in the `intelligems-access-token`\n      request header. Missing or invalid keys return HTTP 401 with body {\"error\":\"Unauthorized\"}.\n    sources: [openapi/intelligems-external-api-openapi.yml]\n  - name: oauth2\n    type: oauth2\n    flow: authorizationCode\n    surface: MCP server (https://ai.intelligems.io/mcp)\n    notes: >-\n      The hosted Intelligems MCP server is OAuth2-authenticated\
  \ against an\n      Intelligems organization account; most tools accept an optional\n      `organization` parameter to scope data access.\n    sources: [mcp/intelligems-mcp.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/authentication/intelligems-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- A/B Testing
- Ecommerce
- Pricing
- Personalization
- Conversion Rate Optimization
- Shopify
- Analytics
- Experimentation
---
