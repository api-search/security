---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Tarx Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: TARXAN Inc declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: TARXAN Inc
provider_slug: tarx-com
scheme_count: 3
schemes:
- anonymous_access: 'Optional for the public-safe subset. initialize, tools/list, prompts/list, resources/list, resources/read (tarx://system/*) and read-only tools such as tarx_status and tarx_skills_list succeed with no credential. tarx_memory_search without a token returns a 200 tool result whose content is {"error":"Authentication required for private memory reads. Provide a Bearer token."} (no 401, no WWW-Authenticate — the challenge is inside the tool payload, which an MCP client''s OAuth discovery will not see). The provider''s mcp.json says auth.required: false, "Public context tools work without auth. Private memory reads and writes require OAuth/Bearer auth."'
  authorization_endpoint: https://mcp.tarx.com/oauth/authorize
  bearer_methods_supported:
  - header
  client_type: 'public (token_endpoint_auth_methods_supported: [none])'
  dynamic_client_registration: false
  evidence:
  - body: '{"error":"invalid_request","error_description":"missing redirect_uri"}'
    http_status: 400
    method: GET
    note: live authorization endpoint
    url: https://mcp.tarx.com/oauth/authorize
  - http_status: 404
    note: no DCR endpoint, consistent with the metadata
    url: https://mcp.tarx.com/register
  - http_status: 404
    note: OAuth 2.0 only, not OIDC
    url: https://mcp.tarx.com/.well-known/openid-configuration
  flow: authorization_code
  id: mcp_oauth2
  issuer: https://mcp.tarx.com
  metadata:
    rfc8414: well-known/tarx-com-oauth-authorization-server.json
    rfc9728: well-known/tarx-com-oauth-protected-resource.json
  pkce: S256 (code_challenge_methods_supported)
  registration_endpoint: null
  resource: https://mcp.tarx.com/mcp
  scopes:
  - public
  - user
  - chatgpt_private_memory
  surface: https://mcp.tarx.com/mcp
  token_endpoint: https://mcp.tarx.com/oauth/token
  type: oauth2
- additional_headers_allowed:
  - X-Request-ID
  - X-TARX-Lease-Token
  anonymous_access: GET /v1/models answers 200 without a key; POST /v1/chat/completions without a key answers 401.
  error_on_missing: 401 {"error":{"message":"Authentication required.","type":"authentication_error","param":null,"code":"tarx_api_key_required"},"request_id":"req_..."}
  evidence:
  - http_status: 200
    method: GET
    url: https://api.tarx.com/v1/models
  - error_code: tarx_api_key_required
    http_status: 401
    method: POST
    url: https://api.tarx.com/v1/chat/completions
  header: Authorization
  id: api_key_bearer
  key_name: TARX API key ("a TARX key and execution policy are enabled for the account" — docs.tarx.com/developers/api)
  key_prefix: null
  obtain: Not self-serve; docs describe hosted capacity as Pilot-ready with keys enabled per account. No key-management page was found.
  scheme: bearer
  surface: https://api.tarx.com/v1
  type: http
- id: courier_open
  note: GET /api/courier/ping, /api/courier/tick and /api/rail/census answer 200 with no credential. POST /api/souls and /api/souls/:id/touch are documented in skill.md with a JSON body and no auth field; GET /api/souls returns 405 (method not allowed). No POST was sent (it creates a record).
  surface: https://tarx.com/api (courier / souls / census)
  type: none
slug: tarx-com-authentication
source_filename: tarx-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: https://mcp.tarx.com/.well-known/oauth-authorization-server + https://mcp.tarx.com/.well-known/oauth-protected-resource + unauthenticated calls to api.tarx.com/v1 and mcp.tarx.com/mcp (2026-09-19)\ndocs: https://docs.tarx.com/developers/api\nnote: >-\n  No OpenAPI declares securitySchemes, so this profile is built from the provider's published OAuth\n  metadata and from observed unauthenticated responses. Three surfaces, three models.\nschemes:\n- id: mcp_oauth2\n  surface: https://mcp.tarx.com/mcp\n  type: oauth2\n  flow: authorization_code\n  pkce: S256 (code_challenge_methods_supported)\n  client_type: \"public (token_endpoint_auth_methods_supported: [none])\"\n  issuer: https://mcp.tarx.com\n  authorization_endpoint: https://mcp.tarx.com/oauth/authorize\n  token_endpoint: https://mcp.tarx.com/oauth/token\n  registration_endpoint: null\n  dynamic_client_registration: false\n  scopes: [public, user, chatgpt_private_memory]\n\
  \  bearer_methods_supported: [header]\n  resource: https://mcp.tarx.com/mcp\n  metadata:\n    rfc8414: well-known/tarx-com-oauth-authorization-server.json\n    rfc9728: well-known/tarx-com-oauth-protected-resource.json\n  anonymous_access: >-\n    Optional for the public-safe subset. initialize, tools/list, prompts/list, resources/list,\n    resources/read (tarx://system/*) and read-only tools such as tarx_status and tarx_skills_list\n    succeed with no credential. tarx_memory_search without a token returns a 200 tool result whose\n    content is {\"error\":\"Authentication required for private memory reads. Provide a Bearer token.\"}\n    (no 401, no WWW-Authenticate — the challenge is inside the tool payload, which an MCP client's\n    OAuth discovery will not see). The provider's mcp.json says auth.required: false, \"Public context\n    tools work without auth. Private memory reads and writes require OAuth/Bearer auth.\"\n  evidence:\n  - {url: https://mcp.tarx.com/oauth/authorize,\
  \ method: GET, http_status: 400, body: '{\"error\":\"invalid_request\",\"error_description\":\"missing redirect_uri\"}', note: live authorization endpoint}\n  - {url: https://mcp.tarx.com/register, http_status: 404, note: 'no DCR endpoint, consistent with the metadata'}\n  - {url: https://mcp.tarx.com/.well-known/openid-configuration, http_status: 404, note: 'OAuth 2.0 only, not OIDC'}\n- id: api_key_bearer\n  surface: https://api.tarx.com/v1\n  type: http\n  scheme: bearer\n  header: Authorization\n  key_name: TARX API key (\"a TARX key and execution policy are enabled for the account\" — docs.tarx.com/developers/api)\n  key_prefix: null\n  obtain: Not self-serve; docs describe hosted capacity as Pilot-ready with keys enabled per account. No key-management page was found.\n  additional_headers_allowed: [X-Request-ID, X-TARX-Lease-Token]\n  anonymous_access: GET /v1/models answers 200 without a key; POST /v1/chat/completions without a key answers 401.\n  error_on_missing: '401 {\"error\"\
  :{\"message\":\"Authentication required.\",\"type\":\"authentication_error\",\"param\":null,\"code\":\"tarx_api_key_required\"},\"request_id\":\"req_...\"}'\n  evidence:\n  - {url: https://api.tarx.com/v1/models, method: GET, http_status: 200}\n  - {url: https://api.tarx.com/v1/chat/completions, method: POST, http_status: 401, error_code: tarx_api_key_required}\n- id: courier_open\n  surface: https://tarx.com/api (courier / souls / census)\n  type: none\n  note: >-\n    GET /api/courier/ping, /api/courier/tick and /api/rail/census answer 200 with no credential.\n    POST /api/souls and /api/souls/:id/touch are documented in skill.md with a JSON body and no auth\n    field; GET /api/souls returns 405 (method not allowed). No POST was sent (it creates a record).\naccount_identity:\n  method: email magic link\n  source: https://tarx.com/terms (\"You sign in with an email magic link. The email address you provide is the canonical identity for your account.\")\nlocal_runtime:\n  surface: http://127.0.0.1:11440\n\
  \  note: The local OpenAI-compatible route and local MCP need no key (\"No account. No API key.\" — howdy.tarx.com); out of scope for a public profile but recorded because the docs' primary examples target it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tarx-com/refs/heads/main/authentication/tarx-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- AI Agents
- Agent Runtime
- Local-First AI
- Private AI
- MCP
- A2A
- LLM
- Inference
- Developer Tools
- Hardware
- Robotics
---
