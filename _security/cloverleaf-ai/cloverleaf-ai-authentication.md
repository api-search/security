---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Cloverleaf Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cloverleaf AI secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cloverleaf AI
provider_slug: cloverleaf-ai
scheme_count: 2
schemes:
- applies_to: https://mcp.cloverleaf.ai/
  challenge_on_missing_token: 'HTTP 401 with WWW-Authenticate: Bearer error="invalid_token", resource_metadata="https://mcp.cloverleaf.ai/.well-known/oauth-protected-resource"'
  flows:
  - authorizationUrl: https://auth.cloverleaf.ai/authorize
    flow: authorizationCode
    refreshUrl: https://auth.cloverleaf.ai/oauth/token
    scopes:
      email: Email address claim
      offline_access: Refresh token issuance
      openid: OpenID Connect authentication
      profile: Basic profile claims
    tokenUrl: https://auth.cloverleaf.ai/oauth/token
  name: mcp-oauth2
  presented_as: 'Authorization: Bearer <access_token>'
  sources:
  - well-known/cloverleaf-ai-oauth-protected-resource.json
  token_type: Bearer
  type: oauth2
- applies_to: https://app.cloverleaf.ai/ (web application sign-in)
  dpop_signing_alg_values_supported:
  - ES256
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.cloverleaf.ai/
  jwks_uri: https://auth.cloverleaf.ai/.well-known/jwks.json
  mfa: true
  name: auth0-oidc
  openIdConnectUrl: https://auth.cloverleaf.ai/.well-known/openid-configuration
  provider: Auth0 (tenant cloverleaf-prod.us.auth0.com)
  sources:
  - well-known/cloverleaf-ai-openid-configuration.json
  type: openIdConnect
  userinfo_endpoint: https://auth.cloverleaf.ai/userinfo
slug: cloverleaf-ai-authentication
source_filename: cloverleaf-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: >-\n  https://mcp.cloverleaf.ai/.well-known/oauth-protected-resource,\n  https://mcp.cloverleaf.ai/.well-known/oauth-authorization-server,\n  https://auth.cloverleaf.ai/.well-known/openid-configuration\n\n# Derived from the live discovery documents, not from an OpenAPI spec — Cloverleaf AI\n# publishes no OpenAPI. This is the authentication contract for the one machine-callable\n# surface the company operates: the MCP server at https://mcp.cloverleaf.ai/.\n\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  bearer_token: true\n  pkce_required_methods: [S256]\n  dynamic_client_registration: true\n  covers: MCP server (https://mcp.cloverleaf.ai/)\n  no_api_key_program: >-\n    No API key or personal access token program is documented anywhere on the public\n    surface. The only observed credential path is the OAuth authorization-code flow\n    against the company's Auth0 tenant.\n\
  \nschemes:\n- name: mcp-oauth2\n  type: oauth2\n  applies_to: https://mcp.cloverleaf.ai/\n  sources: [well-known/cloverleaf-ai-oauth-protected-resource.json]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.cloverleaf.ai/authorize\n    tokenUrl: https://auth.cloverleaf.ai/oauth/token\n    refreshUrl: https://auth.cloverleaf.ai/oauth/token\n    scopes:\n      openid: OpenID Connect authentication\n      profile: Basic profile claims\n      email: Email address claim\n      offline_access: Refresh token issuance\n  token_type: Bearer\n  presented_as: 'Authorization: Bearer <access_token>'\n  challenge_on_missing_token: >-\n    HTTP 401 with WWW-Authenticate: Bearer error=\"invalid_token\",\n    resource_metadata=\"https://mcp.cloverleaf.ai/.well-known/oauth-protected-resource\"\n\n- name: auth0-oidc\n  type: openIdConnect\n  applies_to: https://app.cloverleaf.ai/ (web application sign-in)\n  openIdConnectUrl: https://auth.cloverleaf.ai/.well-known/openid-configuration\n\
  \  sources: [well-known/cloverleaf-ai-openid-configuration.json]\n  issuer: https://auth.cloverleaf.ai/\n  jwks_uri: https://auth.cloverleaf.ai/.well-known/jwks.json\n  userinfo_endpoint: https://auth.cloverleaf.ai/userinfo\n  id_token_signing_alg_values_supported: [HS256, RS256, PS256]\n  dpop_signing_alg_values_supported: [ES256]\n  mfa: true      # mfa_challenge_endpoint advertised\n  provider: Auth0 (tenant cloverleaf-prod.us.auth0.com)\n\nregistration:\n  dynamic: true\n  spec: RFC 7591\n  endpoint: https://auth.cloverleaf.ai/oidc/register\n  note: >-\n    Open dynamic client registration is what lets a generic MCP client (Claude, ChatGPT)\n    connect without a hand-issued client_id. It was observed as advertised metadata only;\n    no registration request was made.\n\nx-evidence:\n- url: https://mcp.cloverleaf.ai/.well-known/oauth-protected-resource\n  http_status: 200\n- url: https://mcp.cloverleaf.ai/.well-known/oauth-authorization-server\n  http_status: 200\n- url: https://auth.cloverleaf.ai/.well-known/openid-configuration\n\
  \  http_status: 200\n- url: https://mcp.cloverleaf.ai/\n  http_status: 401\n  note: anonymous POST returns the Bearer challenge quoted above\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloverleaf-ai/refs/heads/main/authentication/cloverleaf-ai-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Government
- B2G
- Sales Intelligence
- Public Sector
- GovTech
- Procurement
- RFP
- Legislative Intelligence
- Speech to Text
- Artificial Intelligence
---
