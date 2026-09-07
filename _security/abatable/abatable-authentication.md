---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Abatable Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- deviceCode
- implicit
- password
- tokenExchange
- jwtBearer
overview: Abatable secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, deviceCode, implicit, password, tokenExchange, and jwtBearer flow(s).
provider_name: Abatable
provider_slug: abatable
scheme_count: 2
schemes:
- authorization_endpoint: https://login.abatable.com/authorize
  code_challenge_methods_supported:
  - S256
  - plain
  device_authorization_endpoint: https://login.abatable.com/oauth/device/code
  dpop_signing_alg_values_supported:
  - ES256
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  issuer: https://login.abatable.com/
  jwks_uri: https://login.abatable.com/.well-known/jwks.json
  name: Auth0 OIDC (end-user application sign-in)
  observed_client_id_in_login_redirect: 4tYWXA9Pn1WFdKGAtSoKT9fsVwyupxMn
  observed_connection: Username-Password-Authentication
  observed_redirect_uri: https://app.abatable.com/api/auth/callback
  openIdConnectUrl: https://login.abatable.com/.well-known/openid-configuration
  registration_endpoint: https://login.abatable.com/oidc/register
  revocation_endpoint: https://login.abatable.com/oauth/revoke
  sources:
  - well-known/abatable-login-openid-configuration.json
  token_endpoint: https://login.abatable.com/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://login.abatable.com/userinfo
- alternative_client: The Cloudflare Access protected-resource document also advertises `cloudflared access curl` as an interactive authentication method for CLI callers.
  challenge_observed: 'HTTP 401 WWW-Authenticate: Bearer realm="OAuth", error="invalid_token", resource_metadata=...'
  code_challenge_methods_supported:
  - S256
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://abatable.cloudflareaccess.com/cdn-cgi/access/oauth/authorization
    flow: authorizationCode
    refreshUrl: https://abatable.cloudflareaccess.com/cdn-cgi/access/oauth/token
    scopes: {}
    tokenUrl: https://abatable.cloudflareaccess.com/cdn-cgi/access/oauth/token
  issuer: https://abatable.cloudflareaccess.com
  name: Cloudflare Access OAuth (MCP endpoint)
  protected_resource: https://mcp.abatable.com
  registration_endpoint: https://abatable.cloudflareaccess.com/cdn-cgi/access/oauth/registration
  rfc9728: true
  sources:
  - well-known/abatable-mcp-oauth-authorization-server.json
  - well-known/abatable-mcp-oauth-protected-resource.json
  type: oauth2
slug: abatable-authentication
source_filename: abatable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://login.abatable.com/.well-known/openid-configuration and\n  https://mcp.abatable.com/.well-known/oauth-protected-resource — fetched 2026-09-05.\n  No OpenAPI exists in this repo, so nothing here is derived from a spec; every field below was\n  read out of a discovery document the provider serves.\ndocs: null\ndocs_note: >-\n  Abatable publishes no authentication documentation. There is no developer portal and no API\n  reference; /developers on abatable.com is a marketing page for carbon PROJECT developers, not\n  software developers. The auth model below is what the two live discovery surfaces disclose.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken, deviceCode, implicit, password, tokenExchange, jwtBearer]\n  human_auth: OIDC via an Auth0 tenant on the custom domain login.abatable.com\n  machine_auth: OAuth 2.0 via Cloudflare Access\
  \ for the MCP endpoint\n  two_independent_issuers: true\n  note: >-\n    The application and the MCP endpoint do NOT share an identity provider. app.abatable.com\n    authenticates end users against Auth0 (issuer https://login.abatable.com/); mcp.abatable.com is\n    gated by Cloudflare Access (issuer https://abatable.cloudflareaccess.com). An agent holding an\n    application session token cannot call the MCP server with it.\nschemes:\n- name: Auth0 OIDC (end-user application sign-in)\n  type: openIdConnect\n  openIdConnectUrl: https://login.abatable.com/.well-known/openid-configuration\n  issuer: https://login.abatable.com/\n  authorization_endpoint: https://login.abatable.com/authorize\n  token_endpoint: https://login.abatable.com/oauth/token\n  userinfo_endpoint: https://login.abatable.com/userinfo\n  jwks_uri: https://login.abatable.com/.well-known/jwks.json\n  device_authorization_endpoint: https://login.abatable.com/oauth/device/code\n  revocation_endpoint: https://login.abatable.com/oauth/revoke\n\
  \  registration_endpoint: https://login.abatable.com/oidc/register\n  code_challenge_methods_supported: [S256, plain]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  id_token_signing_alg_values_supported: [HS256, RS256, PS256]\n  dpop_signing_alg_values_supported: [ES256]\n  observed_client_id_in_login_redirect: 4tYWXA9Pn1WFdKGAtSoKT9fsVwyupxMn\n  observed_redirect_uri: https://app.abatable.com/api/auth/callback\n  observed_connection: Username-Password-Authentication\n  sources: [well-known/abatable-login-openid-configuration.json]\n- name: Cloudflare Access OAuth (MCP endpoint)\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://abatable.cloudflareaccess.com/cdn-cgi/access/oauth/authorization\n    tokenUrl: https://abatable.cloudflareaccess.com/cdn-cgi/access/oauth/token\n    refreshUrl: https://abatable.cloudflareaccess.com/cdn-cgi/access/oauth/token\n    scopes: {}\n  issuer: https://abatable.cloudflareaccess.com\n\
  \  registration_endpoint: https://abatable.cloudflareaccess.com/cdn-cgi/access/oauth/registration\n  dynamic_client_registration: true\n  code_challenge_methods_supported: [S256]\n  protected_resource: https://mcp.abatable.com\n  challenge_observed: 'HTTP 401 WWW-Authenticate: Bearer realm=\"OAuth\", error=\"invalid_token\", resource_metadata=...'\n  rfc9728: true\n  alternative_client: >-\n    The Cloudflare Access protected-resource document also advertises `cloudflared access curl`\n    as an interactive authentication method for CLI callers.\n  sources:\n  - well-known/abatable-mcp-oauth-authorization-server.json\n  - well-known/abatable-mcp-oauth-protected-resource.json\napi_keys:\n  supported: unknown\n  note: No API key programme is documented or discoverable on any public Abatable surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abatable/refs/heads/main/authentication/abatable-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Carbon Markets
- Carbon Credits
- Carbon Offsets
- Environmental Assets
- Voluntary Carbon Market
- CORSIA
- Climate
- Sustainability
- Net Zero
- Procurement
- Market Intelligence
- Due Diligence
- ESG
- MCP
---
