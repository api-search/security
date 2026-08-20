---
api_key_in:
- header
api_specs:
- filename: intelligems-analytics-api-openapi.yml
  format: yaml
  label: Intelligems Analytics API
  slug: intelligems-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/openapi/intelligems-analytics-api-openapi.yml
- filename: intelligems-experiences-api-openapi.yml
  format: yaml
  label: Intelligems Experiences API
  slug: intelligems-experiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/openapi/intelligems-experiences-api-openapi.yml
- filename: intelligems-holiday-benchmark-api-openapi.yml
  format: yaml
  label: Intelligems Holiday Benchmark API
  slug: intelligems-holiday-benchmark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/openapi/intelligems-holiday-benchmark-api-openapi.yml
- filename: intelligems-custom-events-api-openapi.yml
  format: yaml
  label: Intelligems Custom Events API
  slug: intelligems-custom-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/openapi/intelligems-custom-events-api-openapi.yml
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
  name: intelligems_access_token
  notes: Include your Intelligems-issued API key in the `intelligems-access-token` request header. The key is organization-wide with no scopes and no test/live separation. Missing, empty or invalid keys all return HTTP 401 with body {"error":"Unauthorized"} — the API does not distinguish the three cases.
  parameter_name: intelligems-access-token
  scope_model: none
  sources:
  - openapi/_original/intelligems-external-api-openapi.yml
  - https://docs.intelligems.io/developer-resources/external-api/intelligems-external-api/authentication
  spec_evidence: components.securitySchemes.intelligems_access_token in the OpenAPI Intelligems publishes on its own API-reference pages; applied as a root-level security requirement.
  surface: External API (https://api.intelligems.io)
  type: apiKey
- bearer_methods:
  - header
  dynamic_client_registration: true
  endpoints:
    authorization: https://ai.intelligems.io/oauth/authorize
    issuer: https://ai.intelligems.io
    registration: https://ai.intelligems.io/oauth/register
    token: https://ai.intelligems.io/oauth/token
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  name: mcp-oauth2
  notes: The hosted MCP server is OAuth2-authenticated against an Intelligems organization account and publishes RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata anonymously. Most tools accept an optional `organization` parameter to scope data access; there is no per-tool scope.
  pkce: S256
  scopes:
  - member
  see: scopes/intelligems-scopes.yml
  sources:
  - https://ai.intelligems.io/.well-known/oauth-authorization-server
  - https://ai.intelligems.io/.well-known/oauth-protected-resource
  - mcp/intelligems-mcp.yml
  surface: MCP server (https://ai.intelligems.io/mcp)
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - none
  type: oauth2
slug: intelligems-authentication
source_filename: intelligems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.intelligems.io/developer-resources/external-api/intelligems-external-api/authentication\ndocs: https://docs.intelligems.io/developer-resources/external-api/intelligems-external-api/authentication\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: intelligems_access_token\n    type: apiKey\n    in: header\n    parameter_name: intelligems-access-token\n    surface: External API (https://api.intelligems.io)\n    scope_model: none\n    notes: >-\n      Include your Intelligems-issued API key in the `intelligems-access-token` request\n      header. The key is organization-wide with no scopes and no test/live separation.\n      Missing, empty or invalid keys all return HTTP 401 with body {\"error\":\"Unauthorized\"}\n      — the API does not distinguish the three cases.\n    sources:\n      - openapi/_original/intelligems-external-api-openapi.yml\n \
  \     - https://docs.intelligems.io/developer-resources/external-api/intelligems-external-api/authentication\n    spec_evidence: >-\n      components.securitySchemes.intelligems_access_token in the OpenAPI Intelligems\n      publishes on its own API-reference pages; applied as a root-level security\n      requirement.\n  - name: mcp-oauth2\n    type: oauth2\n    flow: authorizationCode\n    pkce: S256\n    surface: MCP server (https://ai.intelligems.io/mcp)\n    dynamic_client_registration: true\n    endpoints:\n      issuer: https://ai.intelligems.io\n      authorization: https://ai.intelligems.io/oauth/authorize\n      token: https://ai.intelligems.io/oauth/token\n      registration: https://ai.intelligems.io/oauth/register\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [client_secret_post, client_secret_basic, none]\n    scopes: [member]\n    bearer_methods: [header]\n    notes: >-\n      The hosted MCP server is OAuth2-authenticated against\
  \ an Intelligems organization\n      account and publishes RFC 8414 authorization-server metadata and RFC 9728\n      protected-resource metadata anonymously. Most tools accept an optional\n      `organization` parameter to scope data access; there is no per-tool scope.\n    sources:\n      - https://ai.intelligems.io/.well-known/oauth-authorization-server\n      - https://ai.intelligems.io/.well-known/oauth-protected-resource\n      - mcp/intelligems-mcp.yml\n    see: scopes/intelligems-scopes.yml\nwebhook_verification:\n  method: HMAC-SHA256 signature over the payload with a shared secret\n  see: asyncapi/intelligems-webhooks.yml\nx-evidence:\n  - {url: 'https://ai.intelligems.io/.well-known/oauth-authorization-server', status: 200, fetched: '2026-08-13'}\n  - {url: 'https://ai.intelligems.io/mcp', status: 401, fetched: '2026-08-13'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/authentication/intelligems-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- A/B Testing
- E-Commerce
- Pricing
- Personalization
- Conversion Rate Optimization
- Shopify
- Analytics
- Experimentation
- MCP
- Webhook
- Profit Optimization
---
