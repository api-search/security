---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Jasper Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Jasper secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Jasper
provider_slug: jasper
scheme_count: 3
schemes:
- description: Workspace-scoped API token sent in the X-API-KEY request header. Token management is restricted to users with the Admin or Developer role and is done at https://app.jasper.ai/settings/dev-tools/tokens. API access requires the Jasper Business plan.
  in: header
  name: ApiKeyAuth
  parameter_name: X-API-KEY
  type: apiKey
- description: 'OAuth 2.0 authorization-code flow with PKCE (S256) and Dynamic Client Registration, used by the hosted MCP server and agent integrations. Bearer access token sent as Authorization: Bearer.'
  flows:
  - authorizationUrl: https://api.jasper.ai/oauth2/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    introspectionUrl: https://api.jasper.ai/oauth2/introspect
    issuer: https://api.jasper.ai
    pkce: S256
    registrationUrl: https://api.jasper.ai/oauth2/register
    revocationUrl: https://api.jasper.ai/oauth2/revoke
    scopes:
    - mcp
    - user:read
    - user
    - openid
    - email
    - profile
    tokenUrl: https://api.jasper.ai/oauth2/token
    token_endpoint_auth_methods:
    - client_secret_post
    - client_secret_basic
  name: OAuth2
  type: oauth2
- description: OIDC discovery is published; response_types [code], scopes include openid/email/profile.
  name: OpenIDConnect
  openIdConnectUrl: https://api.jasper.ai/.well-known/openid-configuration
  type: openIdConnect
slug: jasper-authentication
source_filename: jasper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://developers.jasper.ai/docs/authentication ;\n  https://api.jasper.ai/.well-known/openid-configuration ;\n  https://api.jasper.ai/.well-known/oauth-authorization-server\ndocs: https://developers.jasper.ai/docs/authentication\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: X-API-KEY\n  description: >-\n    Workspace-scoped API token sent in the X-API-KEY request header. Token management is\n    restricted to users with the Admin or Developer role and is done at\n    https://app.jasper.ai/settings/dev-tools/tokens. API access requires the Jasper Business plan.\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization-code flow with PKCE (S256) and Dynamic Client Registration, used by\n    the hosted MCP server and agent integrations. Bearer access token\
  \ sent as Authorization: Bearer.\n  flows:\n  - flow: authorizationCode\n    issuer: https://api.jasper.ai\n    authorizationUrl: https://api.jasper.ai/oauth2/authorize\n    tokenUrl: https://api.jasper.ai/oauth2/token\n    revocationUrl: https://api.jasper.ai/oauth2/revoke\n    introspectionUrl: https://api.jasper.ai/oauth2/introspect\n    registrationUrl: https://api.jasper.ai/oauth2/register\n    pkce: S256\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n    scopes: [mcp, user:read, user, openid, email, profile]\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://api.jasper.ai/.well-known/openid-configuration\n  description: OIDC discovery is published; response_types [code], scopes include openid/email/profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/authentication/jasper-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Ai Ml
- Artificial Intelligence
- Content Generation
- Marketing
- Generative AI
- Agents
- MCP
---
