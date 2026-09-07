---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dimensions-authentication-api-openapi.yml
  format: yaml
  label: Dimensions Authentication API
  slug: dimensions-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dimensions/refs/heads/main/openapi/dimensions-authentication-api-openapi.yml
- filename: dimensions-query-api-openapi.yml
  format: yaml
  label: Dimensions Query API
  slug: dimensions-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dimensions/refs/heads/main/openapi/dimensions-query-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dimensions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dimensions secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dimensions
provider_slug: dimensions
scheme_count: 2
schemes:
- applies_to:
  - Dimensions Analytics API
  description: Bearer-style JWT obtained from the token exchange. The scheme keyword is literally `JWT`, not `Bearer` — sending `Bearer <token>` fails.
  in: header
  name: jwt
  parameter: Authorization
  sources:
  - openapi/dimensions-authentication-api-openapi.yml
  - openapi/dimensions-query-api-openapi.yml
  - https://docs.dimensions.ai/dsl/api.html
  type: apiKey
  value_format: JWT {token}
- applies_to:
  - Dimensions marketing-site MCP endpoint (https://www.dimensions.ai/wp-json/mcp/mcp-oauth-server)
  authorization_endpoint: https://www.dimensions.ai/oauth/authorize
  flow: authorization_code
  issuer: https://www.dimensions.ai
  name: mcp-oauth
  pkce: S256
  revocation_endpoint: https://www.dimensions.ai/oauth/revoke
  scopes:
  - mcp
  sources:
  - well-known/dimensions-oauth-authorization-server.json
  - well-known/dimensions-oauth-protected-resource.json
  token_endpoint: https://www.dimensions.ai/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: dimensions-authentication
source_filename: dimensions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://docs.dimensions.ai/dsl/api.html (Getting an API Key / Querying the API /\n  API Endpoints), https://docs.dimensions.ai/dsl/faq.html,\n  https://github.com/digital-science/dimensions-analytics-mcp/blob/main/docs/REFERENCE.md,\n  and probed https://www.dimensions.ai/.well-known/oauth-authorization-server\ndocs: https://docs.dimensions.ai/dsl/api.html\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  note: >-\n    Two separate auth surfaces. The Analytics API uses an API key exchanged for a\n    short-lived JWT sent in the Authorization header. The remote MCP endpoint on\n    www.dimensions.ai uses OAuth 2.0 authorization code with PKCE and is unrelated\n    to the Analytics API key.\nschemes:\n- name: jwt\n  type: apiKey\n  in: header\n  parameter: Authorization\n  value_format: 'JWT {token}'\n  description: >-\n    Bearer-style JWT obtained from the token exchange. The scheme keyword is\n\
  \    literally `JWT`, not `Bearer` — sending `Bearer <token>` fails.\n  applies_to:\n  - Dimensions Analytics API\n  sources:\n  - openapi/dimensions-authentication-api-openapi.yml\n  - openapi/dimensions-query-api-openapi.yml\n  - https://docs.dimensions.ai/dsl/api.html\n- name: mcp-oauth\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  issuer: https://www.dimensions.ai\n  authorization_endpoint: https://www.dimensions.ai/oauth/authorize\n  token_endpoint: https://www.dimensions.ai/oauth/token\n  revocation_endpoint: https://www.dimensions.ai/oauth/revoke\n  scopes:\n  - mcp\n  token_endpoint_auth_methods_supported:\n  - none\n  applies_to:\n  - Dimensions marketing-site MCP endpoint (https://www.dimensions.ai/wp-json/mcp/mcp-oauth-server)\n  sources:\n  - well-known/dimensions-oauth-authorization-server.json\n  - well-known/dimensions-oauth-protected-resource.json\ntoken_exchange:\n  step_1:\n    operationId: authenticate\n    method: POST\n    url: https://app.dimensions.ai/api/auth\n\
  \    alt_url: https://app.dimensions.ai/api/auth.json\n    body: '{\"key\": \"<your API key>\"}'\n    content_type: application/json\n    response: '{\"token\": \"<JWT>\"}'\n  step_2:\n    operationId: dslQuery\n    method: POST\n    url: https://app.dimensions.ai/api/dsl/v2\n    header: 'Authorization: JWT {token}'\n    body: a raw DSL query string (text/plain)\n  token_lifetime: approximately 2 hours\n  refresh: no refresh token — re-POST the API key to /api/auth\n  source: https://docs.dimensions.ai/dsl/api.html\nkey_management:\n  issuance: >-\n    Self-service inside the Dimensions web application once the institution has\n    API access — \"My Account\" > settings. Institutional subscription is a\n    prerequisite; there is no self-serve developer signup.\n  key_url: https://app.dimensions.ai/account/settings/general\n  rotation: not documented\n  scopes: none — the Analytics key carries the subscription's entitlements\n  storage_warning: >-\n    The provider's MCP documentation\
  \ warns that MCP client config files store the\n    key in plain text and must never be committed or shared.\n  source: https://docs.dimensions.ai/dsl/mcp.html\nmulti_tenancy:\n  pattern: '<tenant>.dimensions.ai'\n  default_host: https://app.dimensions.ai\n  note: >-\n    Keys are host-scoped. A key issued on a custom instance returns 401\n    Unauthorized against app.dimensions.ai; the base URL must be set to the\n    issuing host (DIMENSIONS_BASE_URL for the MCP server, `endpoint=` for dimcli).\n  source: https://github.com/digital-science/dimensions-analytics-mcp/blob/main/docs/REFERENCE.md\nfailure_modes:\n- status: 401\n  cause: token expired or invalid\n  remedy: mint a new token via /api/auth\n- status: 401\n  cause: key issued on a different Dimensions instance\n  remedy: point the client at the issuing host\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dimensions/refs/heads/main/authentication/dimensions-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Analytics
- Research
- Publications
- Grants
- Patents
- Clinical Trials
- Jupyter Notebooks
- Scientometrics
- Bibliometrics
- Research Intelligence
- Datasets
- Policy Documents
- MCP
---
