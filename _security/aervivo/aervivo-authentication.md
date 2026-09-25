---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Aervivo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aervivo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Aervivo
provider_slug: aervivo
scheme_count: 1
schemes:
- audience: partners, vendors and residents of Aervivo-served communities
  dpop:
    algs:
    - RS256
    - RS384
    - RS512
    - ES256
    - ES384
    - ES512
    - EdDSA
    supported: true
  dynamic_client_registration: true
  endpoints:
    authorization: https://portal.aervivo.com/services/oauth2/authorize
    end_session: https://portal.aervivo.com/services/auth/idp/oidc/logout
    introspection: https://portal.aervivo.com/services/oauth2/introspect
    jwks: https://portal.aervivo.com/id/keys
    registration: https://portal.aervivo.com/services/oauth2/register
    revocation: https://portal.aervivo.com/services/oauth2/revoke
    token: https://portal.aervivo.com/services/oauth2/token
    userinfo: https://portal.aervivo.com/services/oauth2/userinfo
  front_channel_logout: true
  grant_types:
  - authorization_code
  - refresh_token
  id: aervivo-portal-oidc
  id_token_signing_algs:
  - RS256
  issuer: https://portal.aervivo.com
  openIdConnectUrl: https://portal.aervivo.com/.well-known/openid-configuration
  operator: Salesforce Experience Cloud (tenant surface on an Aervivo host)
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  response_types:
  - code
  - token
  - token id_token
  scopes: scopes/aervivo-scopes.yml
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
slug: aervivo-authentication
source_filename: aervivo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: https://portal.aervivo.com/.well-known/openid-configuration\nsummary: >-\n  Aervivo publishes no developer API and no public authentication documentation. The only\n  authentication surface reachable without credentials is the OpenID Connect discovery document\n  for its partner portal at portal.aervivo.com, which is a Salesforce Experience Cloud site\n  running under Aervivo's domain. The issuer is https://portal.aervivo.com, so the endpoints\n  below are Aervivo-hosted, but the flows, scopes and claims are the Salesforce identity\n  platform's, not an Aervivo-designed API auth model.\nschemes:\n- id: aervivo-portal-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://portal.aervivo.com/.well-known/openid-configuration\n  issuer: https://portal.aervivo.com\n  operator: Salesforce Experience Cloud (tenant surface on an Aervivo host)\n  audience: partners, vendors and residents of Aervivo-served communities\n  endpoints:\n\
  \    authorization: https://portal.aervivo.com/services/oauth2/authorize\n    token: https://portal.aervivo.com/services/oauth2/token\n    userinfo: https://portal.aervivo.com/services/oauth2/userinfo\n    jwks: https://portal.aervivo.com/id/keys\n    revocation: https://portal.aervivo.com/services/oauth2/revoke\n    introspection: https://portal.aervivo.com/services/oauth2/introspect\n    registration: https://portal.aervivo.com/services/oauth2/register\n    end_session: https://portal.aervivo.com/services/auth/idp/oidc/logout\n  grant_types: [authorization_code, refresh_token]\n  response_types: [code, token, token id_token]\n  pkce:\n    supported: true\n    code_challenge_methods: [S256]\n  dpop:\n    supported: true\n    algs: [RS256, RS384, RS512, ES256, ES384, ES512, EdDSA]\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic, private_key_jwt]\n  id_token_signing_algs: [RS256]\n  dynamic_client_registration: true\n  front_channel_logout: true\n  scopes: scopes/aervivo-scopes.yml\n\
  public_api_auth: none\ndocs: null\ngaps:\n- No public developer portal, API reference or authentication guide is published on aervivo.com.\n- >-\n  The MCP endpoint at https://www.aervivo.com/_api/mcp accepts anonymous tools/list calls; the\n  Wix visitor-token flow it documents is a Wix platform mechanism, not an Aervivo credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aervivo/refs/heads/main/authentication/aervivo-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Telecommunications
- Internet Service Provider
- Fixed Wireless
- Networking
- Wi-Fi
- OSS BSS
- Connectivity
- Real Estate
- Cloud
---
