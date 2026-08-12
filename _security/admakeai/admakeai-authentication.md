---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Admakeai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AdMakeAI secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AdMakeAI
provider_slug: admakeai
scheme_count: 3
schemes:
- applies_to:
  - REST /api/v1
  - MCP /api/mcp
  constraints:
    expiry: optional
    max_active_keys_per_account: 5
    revocable: true
  in: header
  issued_at: https://admakeai.com/dashboard/integrations/api
  key_prefix: amai_live_
  key_prefix_source: https://github.com/mesmerlord/admakeai-agent-skills README (documented example, not a live key)
  name: apiKey
  parameter: x-api-key
  source: https://admakeai.com/.well-known/mcp.json
  type: apiKey
- name: bearerApiKey
  note: 'The same account API key may be presented as `Authorization: Bearer <key>` instead of `x-api-key`.'
  scheme: bearer
  source: skills/admakeai-api.md
  type: http
- applies_to:
  - MCP /api/mcp
  flows:
  - authorizationUrl: https://admakeai.com/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    registrationUrl: https://admakeai.com/api/oauth/register
    revocationUrl: https://admakeai.com/api/oauth/revoke
    scopes:
    - mcp:read
    - mcp:write
    - mcp:publish
    - offline_access
    tokenUrl: https://admakeai.com/api/oauth/token
  issuer: https://admakeai.com
  name: oauth2
  profile: OAuth 2.1 / MCP authorization
  source: https://admakeai.com/.well-known/oauth-authorization-server
  type: oauth2
slug: admakeai-authentication
source_filename: admakeai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: https://admakeai.com/.well-known/oauth-authorization-server; https://admakeai.com/.well-known/oauth-protected-resource/api/mcp;\n  https://admakeai.com/.well-known/mcp.json; https://github.com/mesmerlord/admakeai-mcp README; skills/admakeai-api.md\ndocs: https://admakeai.com/agents\nnote: >-\n  Derived without an OpenAPI — AdMakeAI publishes no spec, so the security schemes below are read from the provider's\n  own OAuth metadata documents (probed live) and its published MCP server card and agent skill, not from a\n  securitySchemes block. Both surfaces (REST /api/v1 and MCP /api/mcp) sit on one account and one credit pool.\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    applies_to: [REST /api/v1, MCP /api/mcp]\n    issued_at: https://admakeai.com/dashboard/integrations/api\n \
  \   key_prefix: amai_live_\n    key_prefix_source: https://github.com/mesmerlord/admakeai-agent-skills README (documented example, not a live key)\n    constraints:\n      max_active_keys_per_account: 5\n      revocable: true\n      expiry: optional\n    source: https://admakeai.com/.well-known/mcp.json\n  - name: bearerApiKey\n    type: http\n    scheme: bearer\n    note: 'The same account API key may be presented as `Authorization: Bearer <key>` instead of `x-api-key`.'\n    source: skills/admakeai-api.md\n  - name: oauth2\n    type: oauth2\n    profile: OAuth 2.1 / MCP authorization\n    issuer: https://admakeai.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://admakeai.com/oauth/authorize\n        tokenUrl: https://admakeai.com/api/oauth/token\n        revocationUrl: https://admakeai.com/api/oauth/revoke\n        registrationUrl: https://admakeai.com/api/oauth/register\n        pkce: [S256]\n        scopes: [mcp:read, mcp:write, mcp:publish, offline_access]\n\
  \    applies_to: [MCP /api/mcp]\n    source: https://admakeai.com/.well-known/oauth-authorization-server\ndiscovery:\n  authorization_server_metadata: https://admakeai.com/.well-known/oauth-authorization-server\n  protected_resource_metadata: https://admakeai.com/.well-known/oauth-protected-resource/api/mcp\n  specs: [RFC 8414, RFC 9728, RFC 7591, RFC 7636]\n  dynamic_client_registration: true\n  client_id_metadata_document_supported: true\n  token_endpoint_auth_methods_supported: [none, client_secret_post, client_secret_basic]\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code, refresh_token]\n  challenge: >-\n    The provider documents that an unauthenticated MCP call answers 401 with a WWW-Authenticate resource_metadata\n    pointer. This could not be observed from here: an anonymous POST to https://admakeai.com/api/mcp returns HTTP 403\n    with a Cloudflare managed challenge before the application is reached.\nauthorization:\n  model: scope-filtered\
  \ tools\n  detail: >-\n    Scope is enforced at tools/list, not only at call time — a connection approved without mcp:publish never sees the\n    pause/resume tools. Grants are listed and revocable from the dashboard Integrations section.\n  artifact: scopes/admakeai-scopes.yml\nx-evidence:\n  fetched: '2026-08-11'\n  probes:\n    - url: https://admakeai.com/.well-known/oauth-authorization-server\n      http_status: 200\n    - url: https://admakeai.com/.well-known/oauth-protected-resource/api/mcp\n      http_status: 200\n    - url: https://admakeai.com/api/mcp\n      http_status: 403\n      note: Cloudflare managed challenge on an anonymous JSON-RPC POST.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/admakeai/refs/heads/main/authentication/admakeai-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Advertising
- Marketing
- AdTech
- Generative AI
- Image Generation
- Video Generation
- Meta Ads
- Competitive Intelligence
- MCP
- Agents
- Agent Skills
---
