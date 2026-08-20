---
api_key_in: []
api_specs:
- filename: instantly-ai-api-v2-openapi.yml
  format: yaml
  label: Instantly API v2
  slug: instantly-ai-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantly-ai/refs/heads/main/openapi/instantly-ai-api-v2-openapi.yml
- filename: instantly-ai-campaigns-api-openapi.yml
  format: yaml
  label: Instantly Campaigns API
  slug: instantly-ai-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantly-ai/refs/heads/main/openapi/instantly-ai-campaigns-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Instantly Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Instantly secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Instantly
provider_slug: instantly-ai
scheme_count: 2
schemes:
- bearerFormat: API key
  description: 'The primary credential. A workspace API key is created in the Instantly app under Settings > Integrations > API Keys, with the scopes selected at creation time, and is displayed exactly once — it cannot be recovered. Send it as `Authorization: Bearer <key>` on every request. Keys can be listed, created and revoked through the API itself (listAPIKey / createAPIKey / deleteAPIKey).'
  docs: https://developer.instantly.ai/getting-started/authorization
  header: Authorization
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/instantly-ai-api-v2-openapi.yml
  - https://developer.instantly.ai/getting-started/getting-started
  type: http
- description: Instantly runs a full OAuth 2.0 authorization server at https://api.instantly.ai, discoverable anonymously via RFC 8414 metadata. It is not declared in the OpenAPI securitySchemes — it was found by probing /.well-known/oauth-authorization-server — and it is the credential the hosted MCP server at https://mcp.instantly.ai/ challenges for (RFC 9728 protected-resource metadata names api.instantly.ai as its authorization server).
  flows:
  - authorizationUrl: https://api.instantly.ai/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce:
    - S256
    refreshUrl: https://api.instantly.ai/oauth/token
    response_types:
    - code
    scopes: 178
    tokenUrl: https://api.instantly.ai/oauth/token
    token_endpoint_auth_methods:
    - client_secret_post
    - client_secret_basic
    - none
  introspection_endpoint: https://api.instantly.ai/oauth/introspect
  name: OAuth2
  registration_endpoint: https://api.instantly.ai/oauth/register
  revocation_endpoint: https://api.instantly.ai/oauth/revoke
  sources:
  - well-known/instantly-ai-oauth-authorization-server.json
  type: oauth2
slug: instantly-ai-authentication
source_filename: instantly-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/instantly-ai-api-v2-openapi.yml\ndocs: https://developer.instantly.ai/getting-started/authorization\nprobe: https://api.instantly.ai/.well-known/oauth-authorization-server\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - authorizationCode\n  scope_count: 178\n  scopes: scopes/instantly-ai-scopes.yml\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  description: >-\n    The primary credential. A workspace API key is created in the Instantly app under\n    Settings > Integrations > API Keys, with the scopes selected at creation time, and is\n    displayed exactly once — it cannot be recovered. Send it as\n    `Authorization: Bearer <key>` on every request. Keys can be listed, created and\n    revoked through the API itself (listAPIKey / createAPIKey / deleteAPIKey).\n  header: Authorization\n  docs: https://developer.instantly.ai/getting-started/authorization\n\
  \  sources:\n  - openapi/instantly-ai-api-v2-openapi.yml\n  - https://developer.instantly.ai/getting-started/getting-started\n- name: OAuth2\n  type: oauth2\n  description: >-\n    Instantly runs a full OAuth 2.0 authorization server at https://api.instantly.ai,\n    discoverable anonymously via RFC 8414 metadata. It is not declared in the OpenAPI\n    securitySchemes — it was found by probing /.well-known/oauth-authorization-server —\n    and it is the credential the hosted MCP server at https://mcp.instantly.ai/ challenges\n    for (RFC 9728 protected-resource metadata names api.instantly.ai as its authorization\n    server).\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.instantly.ai/oauth/authorize\n    tokenUrl: https://api.instantly.ai/oauth/token\n    refreshUrl: https://api.instantly.ai/oauth/token\n    grant_types:\n    - authorization_code\n    - refresh_token\n    response_types:\n    - code\n    pkce:\n    - S256\n    token_endpoint_auth_methods:\n\
  \    - client_secret_post\n    - client_secret_basic\n    - none\n    scopes: 178\n  registration_endpoint: https://api.instantly.ai/oauth/register\n  revocation_endpoint: https://api.instantly.ai/oauth/revoke\n  introspection_endpoint: https://api.instantly.ai/oauth/introspect\n  sources:\n  - well-known/instantly-ai-oauth-authorization-server.json\nnotes:\n- >-\n  Third-party sender connection is a separate concern: POST /api/v2/oauth/google/init and\n  POST /api/v2/oauth/microsoft/init start a Google/Microsoft OAuth session so a workspace can\n  attach a sending mailbox. Those flows authorize INSTANTLY against Google/Microsoft; they do\n  not authenticate a caller against Instantly. Refresh tokens are never returned by the API.\n  Requires accounts:create to start and accounts:read to poll. See\n  https://developer.instantly.ai/guides/oauth-connection-flow\n- >-\n  Admin workspaces can act on a sub-workspace by adding the `x-as-workspace: <sub_workspace_id>`\n  header alongside the\
  \ bearer token. Documented in the first-party starter kit conventions and\n  advertised in the MCP server's CORS allow-headers.\n- >-\n  There is no separate test/live key namespace and no key prefix convention published, so a key\n  cannot be identified as test-mode from its value.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instantly-ai/refs/heads/main/authentication/instantly-ai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Cold Email
- Outbound
- Sales
- Deliverability
- Lead Database
- Email Verification
- Webhook
---
