---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Augworlds Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Travel World secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Travel World
provider_slug: augworlds-ai
scheme_count: 3
schemes:
- applies_to:
  - https://travel.augworlds.ai/mcp
  authorizationUrl: https://travel.augworlds.ai/api/oauth/authorize
  client_type: public (token_endpoint_auth_methods_supported is [none])
  description: The documented primary path for the MCP server. The client discovers the authorization server from the 401's WWW-Authenticate resource_metadata, registers itself, and runs authorization_code + PKCE with a browser sign-in to a Travel World member account. "There is no token to copy, no --header, and nothing to paste into chat."
  dynamic_client_registration: https://travel.augworlds.ai/api/oauth/register
  flow: authorizationCode
  name: oauth
  pkce: S256 (required — the only code_challenge_method advertised)
  refreshUrl: https://travel.augworlds.ai/api/oauth/token
  revocationUrl: https://travel.augworlds.ai/api/oauth/revoke
  scopes: scopes/augworlds-ai-scopes.yml
  sources:
  - https://augworlds.ai/mcp
  - https://travel.augworlds.ai/.well-known/oauth-authorization-server
  - https://travel.augworlds.ai/.well-known/oauth-protected-resource/mcp
  tokenUrl: https://travel.augworlds.ai/api/oauth/token
  type: oauth2
- applies_to:
  - https://travel.augworlds.ai/mcp
  bearerFormat: opaque token with the tvl_ prefix
  description: Documented fallback for non-interactive callers (CI jobs, servers, scripts, and MCP clients without OAuth support such as Codex). Minted instantly by a member once inside the beta. The docs tell users to read it from an environment variable, never commit it, and never paste it into a chat window.
  name: personal-access-token
  scheme: bearer
  sources:
  - https://augworlds.ai/mcp
  type: http
- applies_to:
  - https://travel.augworlds.ai/a2a
  bearerFormat: Travel World-issued opaque ApiKey bearer token
  description: The A2A agent card's sole security scheme (httpAuthSecurityScheme, scheme Bearer). An unauthenticated JSON-RPC POST returns 401 with error -32001 "Missing or invalid bearer token". The card attaches no scope list, and the OAuth scopes above are published for the MCP resource only.
  name: bearer
  scheme: bearer
  sources:
  - https://travel.augworlds.ai/.well-known/agent-card.json
  type: http
slug: augworlds-ai-authentication
source_filename: augworlds-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://augworlds.ai/mcp\ndocs: https://augworlds.ai/mcp\nspec: null\nsummary:\n  types:\n  - oauth2\n  - http\n  transport: Authorization header, Bearer scheme, HTTPS only\n  note: >-\n    No OpenAPI exists, so derive-authentication.py has nothing to read. The profile was assembled from\n    the public MCP docs page (searched), the RFC 8414 / RFC 9728 discovery documents on\n    travel.augworlds.ai (probed) and the A2A agent card's securitySchemes (probed). Two surfaces, three\n    credential paths.\nschemes:\n- name: oauth\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256 (required — the only code_challenge_method advertised)\n  dynamic_client_registration: https://travel.augworlds.ai/api/oauth/register\n  authorizationUrl: https://travel.augworlds.ai/api/oauth/authorize\n  tokenUrl: https://travel.augworlds.ai/api/oauth/token\n  revocationUrl: https://travel.augworlds.ai/api/oauth/revoke\n  refreshUrl: https://travel.augworlds.ai/api/oauth/token\n\
  \  client_type: public (token_endpoint_auth_methods_supported is [none])\n  scopes: scopes/augworlds-ai-scopes.yml\n  applies_to:\n  - https://travel.augworlds.ai/mcp\n  description: >-\n    The documented primary path for the MCP server. The client discovers the authorization server from the\n    401's WWW-Authenticate resource_metadata, registers itself, and runs authorization_code + PKCE with a\n    browser sign-in to a Travel World member account. \"There is no token to copy, no --header, and nothing\n    to paste into chat.\"\n  sources:\n  - https://augworlds.ai/mcp\n  - https://travel.augworlds.ai/.well-known/oauth-authorization-server\n  - https://travel.augworlds.ai/.well-known/oauth-protected-resource/mcp\n- name: personal-access-token\n  type: http\n  scheme: bearer\n  bearerFormat: opaque token with the tvl_ prefix\n  applies_to:\n  - https://travel.augworlds.ai/mcp\n  description: >-\n    Documented fallback for non-interactive callers (CI jobs, servers, scripts, and MCP clients\
  \ without\n    OAuth support such as Codex). Minted instantly by a member once inside the beta. The docs tell users to\n    read it from an environment variable, never commit it, and never paste it into a chat window.\n  sources:\n  - https://augworlds.ai/mcp\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: Travel World-issued opaque ApiKey bearer token\n  applies_to:\n  - https://travel.augworlds.ai/a2a\n  description: >-\n    The A2A agent card's sole security scheme (httpAuthSecurityScheme, scheme Bearer). An unauthenticated\n    JSON-RPC POST returns 401 with error -32001 \"Missing or invalid bearer token\". The card attaches no\n    scope list, and the OAuth scopes above are published for the MCP resource only.\n  sources:\n  - https://travel.augworlds.ai/.well-known/agent-card.json\ncredentials:\n- id: oauth-access-token\n  header: 'Authorization: Bearer <access_token>'\n  prefix: null\n  use: MCP server via OAuth 2.1 client registration + PKCE (interactive clients)\n\
  - id: personal-access-token\n  header: 'Authorization: Bearer tvl_...'\n  prefix: tvl_\n  use: MCP server from CI, services and non-OAuth clients\n- id: a2a-api-key\n  header: 'Authorization: Bearer <opaque ApiKey>'\n  prefix: null\n  use: A2A JSON-RPC endpoint\naccess_prerequisite: >-\n  Every credential requires a Travel World member account, and membership is invite-only (private beta;\n  free). Signup at https://augworlds.ai/; sign-in at https://travel.augworlds.ai/api/auth/login.\nobserved_challenges:\n- url: https://travel.augworlds.ai/mcp\n  http_status: 401\n  www_authenticate: 'Bearer resource_metadata=\"https://travel.augworlds.ai/.well-known/oauth-protected-resource/mcp\", error=\"invalid_token\"'\n  body: '{\"error\":\"UNAUTHORIZED\"}'\n- url: https://travel.augworlds.ai/a2a\n  http_status: 401\n  body: '{\"jsonrpc\":\"2.0\",\"error\":{\"code\":-32001,\"message\":\"Missing or invalid bearer token\"},\"id\":null}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augworlds-ai/refs/heads/main/authentication/augworlds-ai-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Company
- Travel
- Flights
- Hotels
- Travel Agent
- MCP
- A2A
- AI Agents
- Authentication
- Marketplace
---
