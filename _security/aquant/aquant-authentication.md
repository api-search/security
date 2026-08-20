---
api_key_in:
- body
api_specs:
- filename: aquant-mcp-server-openapi.json
  format: json
  label: Aquant MCP Server
  slug: mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/openapi/aquant-mcp-server-openapi.json
- filename: aquant-voiceai-api-openapi.json
  format: json
  label: Aquant Conversation Platform (VoiceAI) API
  slug: acp-voiceai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/openapi/aquant-voiceai-api-openapi.json
auth_types:
- apiKey
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Aquant Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refreshToken
- password
- deviceCode
overview: Aquant secures its APIs with apiKey, http, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, refreshToken, password, and deviceCode flow(s).
provider_name: Aquant
provider_slug: aquant
scheme_count: 4
schemes:
- api: aquant:acp-voiceai
  documented_errors:
  - code: AUTH_INVALID_CREDENTIALS
    http: 401
    meaning: Invalid API key or secret
  - code: AGENT_NOT_FOUND
    http: 404
    meaning: No agent found for the given agentId
  - code: AGENT_NOT_ACTIVE
    http: 400
    meaning: Agent exists but is not active
  evidence:
    body: '{"status_code":10422,"message":"[{''type'': ''missing'', ''loc'': (''body'', ''api_key''), ...}, {... ''api_secret'' ...}, {... ''agent_id'' ...}]"}'
    http_status: 422
    interpretation: An empty POST returns a field-level validation error naming exactly api_key, api_secret and agent_id as required body fields — confirming the SDK-documented credential exchange against the live endpoint without sending any credential.
    method: POST
    probed: '2026-07-31'
    url: https://voiceai-api.aquant.ai/acp/token
  in: body
  name: acp-key-secret-exchange
  parameters:
  - api_key
  - api_secret
  - agent_id
  produces: bearer access token + agent metadata (agentId, agentName, agentPhone)
  refresh: No refresh endpoint documented. The SDK instructs callers to destroy() the client and re-initialize to obtain a new token.
  token_endpoint: POST https://voiceai-api.aquant.ai/acp/token
  token_ttl_seconds: 3600
  type: apiKey
- api: aquant:acp-voiceai
  applies_to:
  - POST /vss/web-chat
  - WebRTC voice device registration
  bearerFormat: opaque access token
  name: acp-bearer
  obtained_from: POST /acp/token
  scheme: bearer
  type: http
- api: aquant:mcp-server
  evidence:
    oauth_authorization_server: 404
    oauth_protected_resource: 404
    probed: '2026-07-31'
    tools_list_http_status: 200
    url: https://mcp.aquant.ai/mcp
  in: body
  name: mcp-tenant-scope
  note: The MCP server identifies as "Aquant MCP Server (Authenticated)" and every parts tool requires a tenant_id argument (documented in-spec as "[TEMPORARY] The tenant ID. This should be removed in the future."). No bearer/OAuth challenge is issued on tools/list — the tool MANIFEST is anonymous; tool INVOCATION is tenant-scoped.
  parameter: tenant_id
  required_by:
  - part_catalog_lookup
  - part_info
  - part_sources
  type: apiKey
- api: platform (human sign-in, not the public APIs)
  authorizationUrl: https://login.aquant.ai/oauth2/v1/authorize
  deviceAuthorizationUrl: https://login.aquant.ai/oauth2/v1/device/authorize
  dynamic_client_registration: https://login.aquant.ai/oauth2/v1/clients
  endSessionUrl: https://login.aquant.ai/oauth2/v1/logout
  file: well-known/aquant-openid-configuration.json
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  id_token_signing_algs:
  - RS256
  introspectionUrl: https://login.aquant.ai/oauth2/v1/introspect
  issuer: https://login.aquant.ai
  jwksUrl: https://login.aquant.ai/oauth2/v1/keys
  name: aquant-okta-oidc
  openIdConnectUrl: https://login.aquant.ai/.well-known/openid-configuration
  pkce:
  - S256
  provider: Okta
  revocationUrl: https://login.aquant.ai/oauth2/v1/revoke
  scopes:
  - openid
  - email
  - profile
  - address
  - phone
  - offline_access
  - groups
  tokenUrl: https://login.aquant.ai/oauth2/v1/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
  userinfoUrl: https://login.aquant.ai/oauth2/v1/userinfo
slug: aquant-authentication
source_filename: aquant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: >-\n  https://www.npmjs.com/package/@aquantinc/acp-web-sdk (Authentication section),\n  https://login.aquant.ai/.well-known/openid-configuration,\n  live probes of https://voiceai-api.aquant.ai and https://mcp.aquant.ai\ndocs: https://www.npmjs.com/package/@aquantinc/acp-web-sdk#authentication\nnote: >-\n  Neither published OpenAPI declares components.securitySchemes, so the mechanical derive pass\n  (0-working/derive-authentication.py) returns nothing. The auth model below is taken from the\n  first-party SDK documentation and from live, anonymous protocol probes — not guessed.\nsummary:\n  types: [apiKey, http, openIdConnect]\n  api_key_in: [body]\n  oauth2_flows: [authorizationCode, implicit, refreshToken, password, deviceCode]\n  spec_declared_scheme_count: 0\nschemes:\n- name: acp-key-secret-exchange\n  api: aquant:acp-voiceai\n  type: apiKey\n  in: body\n  parameters: [api_key, api_secret, agent_id]\n  token_endpoint:\
  \ POST https://voiceai-api.aquant.ai/acp/token\n  produces: bearer access token + agent metadata (agentId, agentName, agentPhone)\n  token_ttl_seconds: 3600\n  refresh: >-\n    No refresh endpoint documented. The SDK instructs callers to destroy() the client and\n    re-initialize to obtain a new token.\n  evidence:\n    url: https://voiceai-api.aquant.ai/acp/token\n    method: POST\n    probed: '2026-07-31'\n    http_status: 422\n    body: >-\n      {\"status_code\":10422,\"message\":\"[{'type': 'missing', 'loc': ('body', 'api_key'), ...},\n      {... 'api_secret' ...}, {... 'agent_id' ...}]\"}\n    interpretation: >-\n      An empty POST returns a field-level validation error naming exactly api_key, api_secret\n      and agent_id as required body fields — confirming the SDK-documented credential exchange\n      against the live endpoint without sending any credential.\n  documented_errors:\n  - code: AUTH_INVALID_CREDENTIALS\n    http: 401\n    meaning: Invalid API key or secret\n  -\
  \ code: AGENT_NOT_FOUND\n    http: 404\n    meaning: No agent found for the given agentId\n  - code: AGENT_NOT_ACTIVE\n    http: 400\n    meaning: Agent exists but is not active\n- name: acp-bearer\n  api: aquant:acp-voiceai\n  type: http\n  scheme: bearer\n  bearerFormat: opaque access token\n  obtained_from: POST /acp/token\n  applies_to: [POST /vss/web-chat, WebRTC voice device registration]\n- name: mcp-tenant-scope\n  api: aquant:mcp-server\n  type: apiKey\n  in: body\n  parameter: tenant_id\n  required_by: [part_catalog_lookup, part_info, part_sources]\n  note: >-\n    The MCP server identifies as \"Aquant MCP Server (Authenticated)\" and every parts tool\n    requires a tenant_id argument (documented in-spec as \"[TEMPORARY] The tenant ID. This\n    should be removed in the future.\"). No bearer/OAuth challenge is issued on tools/list —\n    the tool MANIFEST is anonymous; tool INVOCATION is tenant-scoped.\n  evidence:\n    url: https://mcp.aquant.ai/mcp\n    probed: '2026-07-31'\n\
  \    tools_list_http_status: 200\n    oauth_protected_resource: 404\n    oauth_authorization_server: 404\n- name: aquant-okta-oidc\n  api: platform (human sign-in, not the public APIs)\n  type: openIdConnect\n  openIdConnectUrl: https://login.aquant.ai/.well-known/openid-configuration\n  issuer: https://login.aquant.ai\n  provider: Okta\n  authorizationUrl: https://login.aquant.ai/oauth2/v1/authorize\n  tokenUrl: https://login.aquant.ai/oauth2/v1/token\n  userinfoUrl: https://login.aquant.ai/oauth2/v1/userinfo\n  jwksUrl: https://login.aquant.ai/oauth2/v1/keys\n  introspectionUrl: https://login.aquant.ai/oauth2/v1/introspect\n  revocationUrl: https://login.aquant.ai/oauth2/v1/revoke\n  endSessionUrl: https://login.aquant.ai/oauth2/v1/logout\n  deviceAuthorizationUrl: https://login.aquant.ai/oauth2/v1/device/authorize\n  dynamic_client_registration: https://login.aquant.ai/oauth2/v1/clients\n  grant_types: [authorization_code, implicit, refresh_token, password, 'urn:ietf:params:oauth:grant-type:device_code']\n\
  \  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, client_secret_jwt, private_key_jwt, none]\n  pkce: [S256]\n  id_token_signing_algs: [RS256]\n  scopes: [openid, email, profile, address, phone, offline_access, groups]\n  file: well-known/aquant-openid-configuration.json\ngaps:\n- >-\n  Neither OpenAPI declares components.securitySchemes, so no security requirement is machine-\n  readable on any of the 13 published operations. Both specs would score zero on\n  securitySchemes-defined and securitySchemes-applied contract-quality checks.\n- >-\n  The MCP server publishes no /.well-known/oauth-protected-resource (RFC 9728), so an MCP\n  client cannot discover how to authenticate tool invocation.\n- >-\n  No public API-key issuance or self-service developer signup — credentials come through the\n  commercial relationship.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/authentication/aquant-authentication.yml
summary_line: apiKey/http/openIdConnect · 4 schemes
tags:
- Company
- Artificial Intelligence
- Agents
- Field Service
- Service Management
- Manufacturing
- Medical Devices
- Industrial Equipment
- Knowledge-Management
- Voice AI
- MCP
- Predictive Maintenance
---
