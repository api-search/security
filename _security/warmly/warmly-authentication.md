---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Warmly Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- deviceCode
- clientCredentials
overview: Warmly secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, deviceCode, and clientCredentials flow(s).
provider_name: Warmly
provider_slug: warmly
scheme_count: 2
schemes:
- description: 'The REST API authenticates with a per-organization API key sent as `Authorization: Bearer $WARMLY_API_KEY` against https://opps-api.getwarmly.com/api. Keys are issued from the Warmly admin UI.'
  evidence:
    body: '{"error":"invalid_token","message":"Missing Bearer token"}'
    http_status: 401
    url: https://opps-api.getwarmly.com/api/agent-tools/tools
  expiry: not published
  key_prefix: not published
  name: RestApiBearer
  rotation_policy: not published
  scheme: bearer
  scopes: []
  type: http
  used_by: REST API (agent-tools endpoints)
- authorization_server: https://vigorous-paper-03.authkit.app
  description: The hosted MCP server at https://opps-api.getwarmly.com/api/mcp is an OAuth 2.0 protected resource. It advertises its authorization server through RFC 9728 protected-resource metadata and returns a compliant WWW-Authenticate challenge, so a standards-aware MCP client discovers the login route with no configuration.
  dynamic_client_registration: true
  endpoints:
    introspection_endpoint: https://vigorous-paper-03.authkit.app/oauth2/introspection
    jwks_uri: https://vigorous-paper-03.authkit.app/oauth2/jwks
    registration_endpoint: https://vigorous-paper-03.authkit.app/oauth2/register
    userinfo_endpoint: https://vigorous-paper-03.authkit.app/oauth2/userinfo
  evidence:
    http_status: 401
    url: https://opps-api.getwarmly.com/api/mcp
    www_authenticate: Bearer resource_metadata="https://opps-api.getwarmly.com/.well-known/oauth-protected-resource", error="invalid_token"
  first_party: false
  first_party_note: A managed AuthKit tenant on a vendor domain. It is treated as Warmly's auth surface because Warmly's own RFC 9728 document at opps-api.getwarmly.com names it as the authorization server for the Warmly MCP resource.
  flows:
  - authorizationUrl: https://vigorous-paper-03.authkit.app/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://vigorous-paper-03.authkit.app/oauth2/token
  - flow: refreshToken
    scope: offline_access
    tokenUrl: https://vigorous-paper-03.authkit.app/oauth2/token
  - deviceAuthorizationUrl: https://vigorous-paper-03.authkit.app/oauth2/device_authorization
    flow: deviceCode
  - flow: clientCredentials
    note: Listed in openid-configuration only.
    tokenUrl: https://vigorous-paper-03.authkit.app/oauth2/token
  id_token_signing_alg: RS256
  name: McpOAuth
  platform: WorkOS AuthKit
  reference: scopes/warmly-scopes.yml
  resource_scopes_supported: []
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  type: oauth2
  used_by: MCP server
slug: warmly-authentication
source_filename: warmly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://help.warmly.ai/articles/9641856032-warmly-technical-documentation-rest-api\ndocs: https://help.warmly.ai/en/collections/5275235549-mcp_api\ndiscovery: https://opps-api.getwarmly.com/.well-known/oauth-protected-resource\nsummary:\n  types: [http, oauth2]\n  http_scheme: bearer\n  oauth2_flows: [authorizationCode, refreshToken, deviceCode, clientCredentials]\n  pkce: [S256]\n  scopes: []\n  org_scoping: [X-Warmly-Organization-Id header, organization_id query param, organizationId body field]\n  note: >-\n    Two different mechanisms for two surfaces: a long-lived per-organization Bearer\n    API key for REST, and delegated OAuth for MCP. Neither carries any scope, so a\n    credential grants everything the organization can do, including the async write\n    tools that mutate a connected CRM.\nschemes:\n- name: RestApiBearer\n  type: http\n  scheme: bearer\n  description: >-\n    The REST API authenticates with a per-organization\
  \ API key sent as\n    `Authorization: Bearer $WARMLY_API_KEY` against https://opps-api.getwarmly.com/api.\n    Keys are issued from the Warmly admin UI.\n  used_by: REST API (agent-tools endpoints)\n  key_prefix: not published\n  rotation_policy: not published\n  expiry: not published\n  scopes: []\n  evidence:\n    url: https://opps-api.getwarmly.com/api/agent-tools/tools\n    http_status: 401\n    body: '{\"error\":\"invalid_token\",\"message\":\"Missing Bearer token\"}'\n- name: McpOAuth\n  type: oauth2\n  description: >-\n    The hosted MCP server at https://opps-api.getwarmly.com/api/mcp is an OAuth 2.0\n    protected resource. It advertises its authorization server through RFC 9728\n    protected-resource metadata and returns a compliant WWW-Authenticate challenge, so\n    a standards-aware MCP client discovers the login route with no configuration.\n  used_by: MCP server\n  authorization_server: https://vigorous-paper-03.authkit.app\n  platform: WorkOS AuthKit\n  first_party: false\n\
  \  first_party_note: >-\n    A managed AuthKit tenant on a vendor domain. It is treated as Warmly's auth\n    surface because Warmly's own RFC 9728 document at opps-api.getwarmly.com names it\n    as the authorization server for the Warmly MCP resource.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://vigorous-paper-03.authkit.app/oauth2/authorize\n    tokenUrl: https://vigorous-paper-03.authkit.app/oauth2/token\n    pkce: S256\n  - flow: refreshToken\n    tokenUrl: https://vigorous-paper-03.authkit.app/oauth2/token\n    scope: offline_access\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://vigorous-paper-03.authkit.app/oauth2/device_authorization\n  - flow: clientCredentials\n    tokenUrl: https://vigorous-paper-03.authkit.app/oauth2/token\n    note: Listed in openid-configuration only.\n  endpoints:\n    jwks_uri: https://vigorous-paper-03.authkit.app/oauth2/jwks\n    introspection_endpoint: https://vigorous-paper-03.authkit.app/oauth2/introspection\n \
  \   userinfo_endpoint: https://vigorous-paper-03.authkit.app/oauth2/userinfo\n    registration_endpoint: https://vigorous-paper-03.authkit.app/oauth2/register\n  dynamic_client_registration: true\n  scopes_supported: [openid, profile, email, offline_access]\n  resource_scopes_supported: []\n  id_token_signing_alg: RS256\n  evidence:\n    url: https://opps-api.getwarmly.com/api/mcp\n    http_status: 401\n    www_authenticate: 'Bearer resource_metadata=\"https://opps-api.getwarmly.com/.well-known/oauth-protected-resource\", error=\"invalid_token\"'\n  reference: scopes/warmly-scopes.yml\norganization_scoping:\n  header: X-Warmly-Organization-Id\n  query_param: organization_id\n  body_field: organizationId\n  note: >-\n    Multi-organization users must scope every call to a single organization. This is\n    tenancy selection, not authorization — it is carried out of band rather than in\n    the token's scope set.\ngaps:\n- No API scopes exist, so least-privilege access to a subset of tools\
  \ is impossible.\n- No API-key prefix, rotation policy or expiry is published.\n- No mutual TLS, no signed requests, no IP allowlisting is documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warmly/refs/heads/main/authentication/warmly-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Sales
- Marketing
- Intent Data
- Revenue Orchestration
- Website Visitor Identification
- AI Agents
- Go-To-Market
- MCP
- Lead Generation
- CRM
---
