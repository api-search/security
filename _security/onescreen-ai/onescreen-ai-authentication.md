---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Onescreen Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: OneScreen AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: OneScreen AI
provider_slug: onescreen-ai
scheme_count: 2
schemes:
- applies_to: https://mcp.onescreen.ai/mcp
  audience_restricted: true
  bearer_methods_supported:
  - header
  challenge:
    header: 'WWW-Authenticate: Bearer resource_metadata="https://mcp.onescreen.ai/.well-known/oauth-protected-resource/mcp"'
    note: A conformant RFC 9728 challenge — an MCP client that has never seen OneScreen can discover the authorization server, register itself dynamically, and complete the flow with no out-of-band configuration. This is the strongest part of OneScreen's posture.
    status: 401
  discovery:
  - spec: RFC 9728
    status: 200
    url: https://mcp.onescreen.ai/.well-known/oauth-protected-resource/mcp
  - spec: RFC 8414
    status: 200
    url: https://mcp.onescreen.ai/.well-known/oauth-authorization-server
  dynamic_client_registration: true
  flows:
    authorization_code:
      authorization_url: https://auth.onescreen.ai/oauth/2.1/authorize
      pkce_required_methods:
      - S256
      refresh_supported: true
      scopes_ref: scopes/onescreen-ai-scopes.yml
      token_url: https://auth.onescreen.ai/oauth/2.1/token
  id: mcp_oauth21
  introspection_endpoint: https://auth.onescreen.ai/oauth/2.1/introspect
  issuer: https://auth.onescreen.ai
  profile: OAuth 2.1
  registration_endpoint: https://auth.onescreen.ai/oauth/2.1/register
  resource_indicator: https://mcp.onescreen.ai/mcp
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
- applies_to: OneScreen web application login
  authorization_url: https://auth.onescreen.ai/propelauth/oauth/authorize
  claims_supported:
  - email
  - email_verified
  - exp
  - first_name
  - last_name
  - iat
  - iss
  - picture_url
  id: propelauth_oidc
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://auth.onescreen.ai
  jwks_uri: https://auth.onescreen.ai/.well-known/jwks.json
  note: Identity-layer login for the product, not the agent surface. Advertises no refresh_token grant, unlike the MCP OAuth 2.1 surface.
  openid_configuration: https://auth.onescreen.ai/.well-known/openid-configuration
  pkce_required_methods:
  - S256
  scopes:
  - openid
  - email
  - profile
  token_url: https://auth.onescreen.ai/propelauth/oauth/token
  type: openIdConnect
  userinfo_url: https://auth.onescreen.ai/propelauth/oauth/userinfo
  vendor: PropelAuth
slug: onescreen-ai-authentication
source_filename: onescreen-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://mcp.onescreen.ai/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.onescreen.ai/.well-known/oauth-authorization-server\ndocs: https://www.onescreen.ai/mcp/\nnote: >-\n  Derived from live OAuth/OIDC discovery documents, not from an OpenAPI securitySchemes block\n  — OneScreen publishes no REST contract. Two distinct authorization surfaces exist on the\n  same issuer host and should not be conflated: the OAuth 2.1 endpoints under\n  /oauth/2.1/ that the MCP server delegates to, and a PropelAuth-hosted OpenID Connect\n  surface under /propelauth/oauth/ used for end-user login to the OneScreen app.\nsummary:\n  scheme_count: 1\n  primary: oauth2\n  api_keys: false\n  mtls: false\n  anonymous_access: false\nschemes:\n- id: mcp_oauth21\n  type: oauth2\n  profile: OAuth 2.1\n  applies_to: https://mcp.onescreen.ai/mcp\n  flows:\n    authorization_code:\n      authorization_url: https://auth.onescreen.ai/oauth/2.1/authorize\n      token_url: https://auth.onescreen.ai/oauth/2.1/token\n   \
  \   refresh_supported: true\n      pkce_required_methods:\n      - S256\n      scopes_ref: scopes/onescreen-ai-scopes.yml\n  issuer: https://auth.onescreen.ai\n  registration_endpoint: https://auth.onescreen.ai/oauth/2.1/register\n  introspection_endpoint: https://auth.onescreen.ai/oauth/2.1/introspect\n  dynamic_client_registration: true\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  bearer_methods_supported:\n  - header\n  audience_restricted: true\n  resource_indicator: https://mcp.onescreen.ai/mcp\n  discovery:\n  - url: https://mcp.onescreen.ai/.well-known/oauth-protected-resource/mcp\n    spec: RFC 9728\n    status: 200\n  - url: https://mcp.onescreen.ai/.well-known/oauth-authorization-server\n    spec: RFC 8414\n    status: 200\n  challenge:\n    status: 401\n    header: 'WWW-Authenticate: Bearer resource_metadata=\"https://mcp.onescreen.ai/.well-known/oauth-protected-resource/mcp\"'\n    note: >-\n      A conformant RFC 9728 challenge\
  \ — an MCP client that has never seen OneScreen can\n      discover the authorization server, register itself dynamically, and complete the flow\n      with no out-of-band configuration. This is the strongest part of OneScreen's posture.\n- id: propelauth_oidc\n  type: openIdConnect\n  applies_to: OneScreen web application login\n  openid_configuration: https://auth.onescreen.ai/.well-known/openid-configuration\n  issuer: https://auth.onescreen.ai\n  authorization_url: https://auth.onescreen.ai/propelauth/oauth/authorize\n  token_url: https://auth.onescreen.ai/propelauth/oauth/token\n  userinfo_url: https://auth.onescreen.ai/propelauth/oauth/userinfo\n  jwks_uri: https://auth.onescreen.ai/.well-known/jwks.json\n  id_token_signing_alg_values_supported:\n  - RS256\n  scopes:\n  - openid\n  - email\n  - profile\n  claims_supported:\n  - email\n  - email_verified\n  - exp\n  - first_name\n  - last_name\n  - iat\n  - iss\n  - picture_url\n  pkce_required_methods:\n  - S256\n  vendor: PropelAuth\n\
  \  note: >-\n    Identity-layer login for the product, not the agent surface. Advertises no refresh_token\n    grant, unlike the MCP OAuth 2.1 surface.\naccess:\n  model: request-access\n  form: https://www.onescreen.ai/mcp/\n  note: >-\n    Dynamic client registration is open, but a OneScreen account must first be approved\n    through the beta waitlist; the provider states verified work domains are usually cleared\n    the same business day.\nsources:\n- https://mcp.onescreen.ai/.well-known/oauth-authorization-server\n- https://mcp.onescreen.ai/.well-known/oauth-protected-resource/mcp\n- https://auth.onescreen.ai/.well-known/openid-configuration\n- https://www.onescreen.ai/mcp/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onescreen-ai/refs/heads/main/authentication/onescreen-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Advertising
- Out-of-Home
- DOOH
- Advertising Technology
- Marketing
- Media
- AI Agents
- MCP
- OAuth
- Agent Readiness
---
