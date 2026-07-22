---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Prelude Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
overview: Prelude secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, and refreshToken flow(s).
provider_name: Prelude
provider_slug: prelude
scheme_count: 1
schemes:
- authorization_endpoint: https://auth-web.dashboard.originhq.com/oauth2/authorize
  bearer_methods_supported:
  - header
  device_authorization_endpoint: https://auth-web.dashboard.originhq.com/oauth2/device_authorization
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://auth-web.dashboard.originhq.com/oauth2/introspection
  issuer: https://auth-web.dashboard.originhq.com
  jwks_uri: https://auth-web.dashboard.originhq.com/oauth2/jwks
  name: OriginOAuth2
  profile: OAuth 2.1
  protected_resource: https://mcp.prod.originhq.com/mcp
  response_types_supported:
  - code
  sources:
  - well-known/prelude-oauth-authorization-server.json
  - well-known/prelude-oauth-protected-resource.json
  token_endpoint: https://auth-web.dashboard.originhq.com/oauth2/token
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
  userinfo_endpoint: https://auth-web.dashboard.originhq.com/oauth2/userinfo
slug: prelude-authentication
source_filename: prelude-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://support.originhq.com/docs/origin-mcp-server\ndocs: https://support.originhq.com/docs/origin-mcp-server\nnote: >-\n  No public REST OpenAPI is published; the auth model below is captured from the hosted MCP\n  server docs and the live OAuth authorization-server / protected-resource metadata.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, refreshToken]\n  dynamic_client_registration: true\n  identity_provider: WorkOS AuthKit (Origin account)\nschemes:\n- name: OriginOAuth2\n  type: oauth2\n  profile: OAuth 2.1\n  issuer: https://auth-web.dashboard.originhq.com\n  authorization_endpoint: https://auth-web.dashboard.originhq.com/oauth2/authorize\n  token_endpoint: https://auth-web.dashboard.originhq.com/oauth2/token\n  device_authorization_endpoint: https://auth-web.dashboard.originhq.com/oauth2/device_authorization\n  introspection_endpoint: https://auth-web.dashboard.originhq.com/oauth2/introspection\n\
  \  userinfo_endpoint: https://auth-web.dashboard.originhq.com/oauth2/userinfo\n  jwks_uri: https://auth-web.dashboard.originhq.com/oauth2/jwks\n  grant_types_supported: [authorization_code, client_credentials, refresh_token, \"urn:ietf:params:oauth:grant-type:device_code\"]\n  response_types_supported: [code]\n  token_endpoint_auth_methods_supported: [none, client_secret_basic, client_secret_post]\n  id_token_signing_alg_values_supported: [RS256]\n  bearer_methods_supported: [header]\n  protected_resource: https://mcp.prod.originhq.com/mcp\n  sources:\n  - well-known/prelude-oauth-authorization-server.json\n  - well-known/prelude-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prelude/refs/heads/main/authentication/prelude-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Cybersecurity
- AI Security
- AI Observability
- Endpoint Security
- AI Agents
- Model Context Protocol
- MCP
- Insight Partners
---
