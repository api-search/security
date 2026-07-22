---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Prox Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- refreshToken
overview: Prox secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, and refreshToken flow(s).
provider_name: Prox
provider_slug: prox
scheme_count: 2
schemes:
- bearer_methods:
  - header
  client_id_metadata_document_supported: true
  code_challenge_methods:
  - S256
  dynamic_client_registration: true
  endpoints:
    introspection: https://signin.useprox.com/oauth2/introspection
    jwks_uri: https://signin.useprox.com/oauth2/jwks
    registration: https://signin.useprox.com/oauth2/register
    userinfo: https://signin.useprox.com/oauth2/userinfo
  flows:
  - authorizationUrl: https://signin.useprox.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://signin.useprox.com/oauth2/token
  - deviceAuthorizationUrl: https://signin.useprox.com/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://signin.useprox.com/oauth2/token
  - flow: refreshToken
    tokenUrl: https://signin.useprox.com/oauth2/token
  issuer: https://signin.useprox.com
  name: OAuth2
  resource: https://mcp.useprox.com
  scopes:
  - openid
  - profile
  - email
  - offline_access
  source: https://mcp.useprox.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
- id_token_signing_alg:
  - RS256
  name: OpenIDConnect
  openIdConnectUrl: https://signin.useprox.com/.well-known/openid-configuration
  source: https://signin.useprox.com/.well-known/openid-configuration
  subject_types:
  - public
  type: openIdConnect
slug: prox-authentication
source_filename: prox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://useprox.com/docs/mcp\ndocs: https://useprox.com/docs/mcp\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, deviceCode, refreshToken]\n  api_key_in: []\n  notes: >-\n    Prox exposes no API keys. Its hosted MCP server is protected by OAuth 2.1\n    (PKCE / S256) with dynamic client registration, delegated to WorkOS AuthKit\n    at signin.useprox.com. Access tokens are presented as bearer tokens in the\n    Authorization header and scoped to the signed-in user's workspace.\nschemes:\n  - name: OAuth2\n    type: oauth2\n    source: https://mcp.useprox.com/.well-known/oauth-authorization-server\n    issuer: https://signin.useprox.com\n    resource: https://mcp.useprox.com\n    bearer_methods: [header]\n    code_challenge_methods: [S256]\n    dynamic_client_registration: true\n    client_id_metadata_document_supported: true\n    flows:\n      - flow: authorizationCode\n        authorizationUrl:\
  \ https://signin.useprox.com/oauth2/authorize\n        tokenUrl: https://signin.useprox.com/oauth2/token\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://signin.useprox.com/oauth2/device_authorization\n        tokenUrl: https://signin.useprox.com/oauth2/token\n      - flow: refreshToken\n        tokenUrl: https://signin.useprox.com/oauth2/token\n    endpoints:\n      registration: https://signin.useprox.com/oauth2/register\n      introspection: https://signin.useprox.com/oauth2/introspection\n      jwks_uri: https://signin.useprox.com/oauth2/jwks\n      userinfo: https://signin.useprox.com/oauth2/userinfo\n    token_endpoint_auth_methods: [none, client_secret_post, client_secret_basic]\n    scopes: [openid, profile, email, offline_access]\n  - name: OpenIDConnect\n    type: openIdConnect\n    source: https://signin.useprox.com/.well-known/openid-configuration\n    openIdConnectUrl: https://signin.useprox.com/.well-known/openid-configuration\n    id_token_signing_alg:\
  \ [RS256]\n    subject_types: [public]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prox/refs/heads/main/authentication/prox-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Artificial Intelligence
- MCP
- Model Context Protocol
- Manufacturing
- Product Support
- Knowledge Base
- Documentation
- Agents
---
