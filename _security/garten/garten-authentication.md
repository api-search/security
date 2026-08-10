---
api_key_in:
- unspecified
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: probed
name: Garten Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Garten secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Garten
provider_slug: garten
scheme_count: 2
schemes:
- applies_to: https://tv.garten.co/mcp
  bearer_methods_supported:
  - header
  code_challenge_methods_supported:
  - S256
  endpoints:
    authorization: https://tv.garten.co/oauth/authorize
    introspection: https://tv.garten.co/oauth/introspect
    registration: https://tv.garten.co/oauth/register
    revocation: https://tv.garten.co/oauth/revoke
    token: https://tv.garten.co/oauth/token
  flows:
  - authorizationUrl: https://tv.garten.co/oauth/authorize
    flow: authorizationCode
    scope_count: 7
    tokenUrl: https://tv.garten.co/oauth/token
  - flow: refreshToken
    tokenUrl: https://tv.garten.co/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://tv.garten.co
  name: garten TV OAuth 2.1
  resource_indicators_supported: true
  response_types_supported:
  - code
  sources:
  - well-known/garten-tv-oauth-authorization-server.json
  - well-known/garten-tv-oauth-protected-resource.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
- applies_to: https://api.garten.co/api/v1, https://api.garten.co/api/v2, https://client.garten.co
  documented: false
  in: unspecified
  name: garten client commerce API key
  observed_behaviour: Anonymous GET of /api/v1/products, /api/v2/storefront/products, /api/v2/storefront/menus and /api/v2/platform/products all return HTTP 401 with body {"error":"You must specify an API key."} — the Spree/Solidus default. garten publishes no documentation, no key-issuance flow and no header/parameter name for this credential, so the location of the key is recorded as unspecified rather than guessed.
  parameter_name: unspecified
  sources:
  - live probe
  type: apiKey
slug: garten-authentication
source_filename: garten-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://tv.garten.co/.well-known/oauth-authorization-server\nnote: 'Derived from live OAuth discovery metadata rather than from an OpenAPI document\n  — garten publishes no machine-readable REST contract. Two distinct authentication\n  surfaces exist in the estate and both are recorded: the OAuth 2.1 surface on garten\n  TV (fully documented by its own metadata) and the opaque API-key surface on the Spree/Solidus\n  client application (observed only through its 401 body; garten publishes no documentation\n  for it, so nothing beyond the observed behaviour is asserted).'\nsummary:\n  types: [oauth2, apiKey]\n  oauth2_flows: [authorizationCode, refreshToken]\n  pkce: [S256]\n  dynamic_client_registration: true\n  api_key_in: [unspecified]\nschemes:\n- name: garten TV OAuth 2.1\n  type: oauth2\n  applies_to: https://tv.garten.co/mcp\n  issuer: https://tv.garten.co\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://tv.garten.co/oauth/authorize\n\
  \    tokenUrl: https://tv.garten.co/oauth/token\n    scope_count: 7\n  - flow: refreshToken\n    tokenUrl: https://tv.garten.co/oauth/token\n  endpoints:\n    authorization: https://tv.garten.co/oauth/authorize\n    token: https://tv.garten.co/oauth/token\n    revocation: https://tv.garten.co/oauth/revoke\n    introspection: https://tv.garten.co/oauth/introspect\n    registration: https://tv.garten.co/oauth/register\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code, refresh_token]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, none]\n  resource_indicators_supported: true\n  bearer_methods_supported: [header]\n  sources: [well-known/garten-tv-oauth-authorization-server.json, well-known/garten-tv-oauth-protected-resource.json]\n- name: garten client commerce API key\n  type: apiKey\n  applies_to: https://api.garten.co/api/v1, https://api.garten.co/api/v2, https://client.garten.co\n\
  \  in: unspecified\n  parameter_name: unspecified\n  documented: false\n  observed_behaviour: 'Anonymous GET of /api/v1/products, /api/v2/storefront/products,\n    /api/v2/storefront/menus and /api/v2/platform/products all return HTTP 401 with\n    body {\"error\":\"You must specify an API key.\"} — the Spree/Solidus default. garten\n    publishes no documentation, no key-issuance flow and no header/parameter name for\n    this credential, so the location of the key is recorded as unspecified rather than\n    guessed.'\n  sources: [live probe]\nposture:\n  strengths:\n  - RFC 8414 authorization-server metadata published and anonymous\n  - RFC 9728 protected-resource metadata published, correctly referenced from the WWW-Authenticate\n    header on a 401\n  - PKCE S256 required-capable; no implicit or password grants advertised\n  - RFC 7591 dynamic client registration endpoint advertised\n  - RFC 8707 resource indicators supported\n  - separate revocation and introspection endpoints advertised\n\
  \  gaps:\n  - no OpenID Connect discovery document (/.well-known/openid-configuration returns\n    404), so there is no id_token / userinfo contract\n  - no human-readable authentication documentation anywhere on garten's public surface\n  - the commerce API-key surface is undocumented — no key issuance, rotation or scoping\n    guidance is published\n  - the OAuth surface covers only the garten TV property, not the core kitchen/market/catering\n    business\nx-evidence:\n- {fetched: '2026-08-04', url: 'https://tv.garten.co/.well-known/oauth-authorization-server',\n   http_status: 200}\n- {fetched: '2026-08-04', url: 'https://tv.garten.co/mcp', http_status: 401, header: www-authenticate}\n- {fetched: '2026-08-04', url: 'https://api.garten.co/api/v2/storefront/products', http_status: 401}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/garten/refs/heads/main/authentication/garten-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Food Service
- Corporate Wellness
- Workplace
- Catering
- Employee Benefits
- Micro Market
- Facilities Management
- Hospitality
- Streaming Video
- MCP
---
