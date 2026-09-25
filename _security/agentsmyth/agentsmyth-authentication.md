---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Agentsmyth Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentSmyth declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AgentSmyth
provider_slug: agentsmyth
scheme_count: 2
schemes:
- flows:
    authorizationCode:
      authorizationUrl: https://app.auth.agentsmyth.com/oauth2/authorize
      pkce: S256
      pkce_required_methods:
      - S256
      refreshUrl: https://app.auth.agentsmyth.com/oauth2/token
      tokenUrl: https://app.auth.agentsmyth.com/oauth2/token
    clientCredentials:
      note: Advertised in the OIDC discovery document's grant_types_supported. This is the machine-to-machine path an agent would use without a human in the loop.
      tokenUrl: https://app.auth.agentsmyth.com/oauth2/token
    deviceCode:
      deviceAuthorizationUrl: https://app.auth.agentsmyth.com/oauth2/device_authorization
      grant: urn:ietf:params:oauth:grant-type:device_code
      tokenUrl: https://app.auth.agentsmyth.com/oauth2/token
  header: Authorization
  in: header
  issuer: https://app.auth.agentsmyth.com
  key: oauth2
  scheme: Bearer
  scopes:
  - openid
  - profile
  - email
  - offline_access
  type: oauth2
- id_token_signing_alg_values_supported:
  - RS256
  key: openIdConnect
  openIdConnectUrl: https://app.auth.agentsmyth.com/.well-known/openid-configuration
  subject_types_supported:
  - public
  type: openIdConnect
  userinfo_endpoint: https://app.auth.agentsmyth.com/oauth2/userinfo
slug: agentsmyth-authentication
source_filename: agentsmyth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: >-\n  https://app.auth.agentsmyth.com/.well-known/openid-configuration and\n  https://api.agentsmyth.com/.well-known/oauth-protected-resource/mcp\nnote: >-\n  Derived entirely from the provider's own live discovery documents, not from an OpenAPI - no\n  OpenAPI is published. There is no public human-readable authentication page; the auth model below\n  is what the machine-readable metadata states.\nsummary: >-\n  OAuth 2.1 / OpenID Connect. The API host api.agentsmyth.com delegates to a WorkOS AuthKit\n  authorization server at app.auth.agentsmyth.com. Bearer access tokens are presented to the\n  protected resource; unauthenticated calls get an RFC 9728 challenge pointing at the\n  protected-resource metadata.\nschemes:\n- key: oauth2\n  type: oauth2\n  in: header\n  header: Authorization\n  scheme: Bearer\n  issuer: https://app.auth.agentsmyth.com\n  flows:\n    authorizationCode:\n      authorizationUrl: https://app.auth.agentsmyth.com/oauth2/authorize\n\
  \      tokenUrl: https://app.auth.agentsmyth.com/oauth2/token\n      refreshUrl: https://app.auth.agentsmyth.com/oauth2/token\n      pkce: S256\n      pkce_required_methods:\n      - S256\n    clientCredentials:\n      tokenUrl: https://app.auth.agentsmyth.com/oauth2/token\n      note: >-\n        Advertised in the OIDC discovery document's grant_types_supported. This is the\n        machine-to-machine path an agent would use without a human in the loop.\n    deviceCode:\n      deviceAuthorizationUrl: https://app.auth.agentsmyth.com/oauth2/device_authorization\n      tokenUrl: https://app.auth.agentsmyth.com/oauth2/token\n      grant: urn:ietf:params:oauth:grant-type:device_code\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n- key: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://app.auth.agentsmyth.com/.well-known/openid-configuration\n  userinfo_endpoint: https://app.auth.agentsmyth.com/oauth2/userinfo\n  id_token_signing_alg_values_supported:\n\
  \  - RS256\n  subject_types_supported:\n  - public\nendpoints:\n  authorization: https://app.auth.agentsmyth.com/oauth2/authorize\n  token: https://app.auth.agentsmyth.com/oauth2/token\n  device_authorization: https://app.auth.agentsmyth.com/oauth2/device_authorization\n  introspection: https://app.auth.agentsmyth.com/oauth2/introspection\n  userinfo: https://app.auth.agentsmyth.com/oauth2/userinfo\n  jwks: https://app.auth.agentsmyth.com/oauth2/jwks\n  registration: https://app.auth.agentsmyth.com/oauth2/register\nclient_registration:\n  dynamic: true\n  endpoint: https://app.auth.agentsmyth.com/oauth2/register\n  spec: RFC 7591\n  client_id_metadata_document_supported: true\n  token_endpoint_auth_methods_supported:\n  - none\n  - client_secret_basic\n  - client_secret_post\n  note: >-\n    Open dynamic client registration plus a \"none\" auth method means a public MCP client can\n    register itself and complete a PKCE authorization-code flow without a pre-provisioned secret.\napi_keys:\n\
  \  supported: false\n  note: No API-key scheme is advertised in any discovery document and none is documented publicly.\nprotected_resources:\n- resource: https://api.agentsmyth.com/mcp\n  metadata: https://api.agentsmyth.com/.well-known/oauth-protected-resource/mcp\n  authorization_servers:\n  - https://app.auth.agentsmyth.com\n  spec: RFC 9728\nx-evidence:\n  fetched: '2026-09-12'\n  probes:\n  - url: https://app.auth.agentsmyth.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://app.auth.agentsmyth.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://api.agentsmyth.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://api.agentsmyth.com/.well-known/oauth-protected-resource/mcp\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentsmyth/refs/heads/main/authentication/agentsmyth-authentication.yml
summary_line: 2 schemes
tags:
- Financial Services
- Capital Markets
- Artificial Intelligence
- AI Agents
- Trading
- Investment Research
- Market Intelligence
- MCP
- Agent-Native
- Fintech
---
