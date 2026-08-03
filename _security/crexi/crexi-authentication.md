---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Crexi Authentication
name_suffix: Authentication
oauth_flows:
- password
- refresh_token
- switch_user
- single_use_token_exchange
overview: CREXi secures its APIs with apiKey, http, oauth2, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password, refresh_token, switch_user, and single_use_token_exchange flow(s).
provider_name: CREXi
provider_slug: crexi
scheme_count: 5
schemes:
- api: crexi-exchange-api
  description: Enter your api key
  evidence: The Swagger UI login page served at https://exchange.crexi.com/ stores the credential as {"ApiKey":{"name":"ApiKey","schema":{"type":"apiKey","description":"Enter your api key","name":"x-api-key","in":"header"}}} — a verbatim OpenAPI apiKey security scheme published in the page's auth.js.
  in: header
  name: ExchangeApiKey
  parameter_name: x-api-key
  sources:
  - https://exchange.crexi.com/Content/auth.js
  type: apiKey
- api: crexi-platform-api
  description: The Swashbuckle Swagger UI and its spec document on the platform API host are protected by HTTP Basic authentication.
  evidence: 'HTTP/2 401 with response header `www-authenticate: Basic` observed 2026-08-01.'
  name: SwaggerUiBasic
  scheme: basic
  sources:
  - https://api.crexi.com/swagger/v1/swagger.json
  type: http
- api: crexi-platform-api
  grant_types_supported:
  - password
  - switch_user
  - single_use_token_exchange
  - refresh_token
  issuer: https://api.crexi.com/
  jwks_uri: https://api.crexi.com/.well-known/jwks
  name: CrexiOAuth2
  scopes_supported:
  - openid
  - offline_access
  sources:
  - well-known/crexi-oauth-authorization-server.json
  token_endpoint: https://api.crexi.com/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - private_key_jwt
  - client_secret_basic
  type: oauth2
- api: crexi-platform-api
  claims_supported:
  - aud
  - exp
  - iat
  - iss
  - sub
  id_token_signing_alg_values_supported:
  - RS256
  name: CrexiOpenIDConnect
  openIdConnectUrl: https://api.crexi.com/.well-known/openid-configuration
  prompt_values_supported:
  - consent
  - login
  - none
  - select_account
  sources:
  - well-known/crexi-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
- api: crexi-listing-api
  description: CREXi issues an API token to each qualifying Listing API partner during onboarding. The help centre documents token issuance but publishes neither the transport (header/query) nor the parameter name.
  gated: true
  in: unknown
  name: ListingApiToken
  sources:
  - https://learn.crexi.com/listing-api-overview-crexi-help-center
  type: apiKey
slug: crexi-authentication
source_filename: crexi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://api.crexi.com/.well-known/openid-configuration\ndocs: https://learn.crexi.com/listing-api-overview-crexi-help-center\nnote: 'Derived from live discovery documents and from the published Swagger UI login\n  script on the Exchange API gateway, not from an OpenAPI securitySchemes block — no\n  CREXi OpenAPI document is publicly retrievable (every spec URL found is auth-gated).'\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - password\n  - refresh_token\n  - switch_user\n  - single_use_token_exchange\nschemes:\n- name: ExchangeApiKey\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: Enter your api key\n  api: crexi-exchange-api\n  sources:\n  - https://exchange.crexi.com/Content/auth.js\n  evidence: 'The Swagger UI login page served at https://exchange.crexi.com/ stores\n    the credential as {\"ApiKey\":{\"name\":\"ApiKey\"\
  ,\"schema\":{\"type\":\"apiKey\",\"description\":\"Enter\n    your api key\",\"name\":\"x-api-key\",\"in\":\"header\"}}} — a verbatim OpenAPI apiKey security\n    scheme published in the page''s auth.js.'\n- name: SwaggerUiBasic\n  type: http\n  scheme: basic\n  api: crexi-platform-api\n  description: The Swashbuckle Swagger UI and its spec document on the platform API\n    host are protected by HTTP Basic authentication.\n  sources:\n  - https://api.crexi.com/swagger/v1/swagger.json\n  evidence: 'HTTP/2 401 with response header `www-authenticate: Basic` observed 2026-08-01.'\n- name: CrexiOAuth2\n  type: oauth2\n  api: crexi-platform-api\n  issuer: https://api.crexi.com/\n  token_endpoint: https://api.crexi.com/token\n  jwks_uri: https://api.crexi.com/.well-known/jwks\n  grant_types_supported:\n  - password\n  - switch_user\n  - single_use_token_exchange\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - private_key_jwt\n  - client_secret_basic\n\
  \  scopes_supported:\n  - openid\n  - offline_access\n  sources:\n  - well-known/crexi-oauth-authorization-server.json\n- name: CrexiOpenIDConnect\n  type: openIdConnect\n  api: crexi-platform-api\n  openIdConnectUrl: https://api.crexi.com/.well-known/openid-configuration\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  claims_supported:\n  - aud\n  - exp\n  - iat\n  - iss\n  - sub\n  prompt_values_supported:\n  - consent\n  - login\n  - none\n  - select_account\n  sources:\n  - well-known/crexi-openid-configuration.json\n- name: ListingApiToken\n  type: apiKey\n  api: crexi-listing-api\n  in: unknown\n  description: 'CREXi issues an API token to each qualifying Listing API partner during\n    onboarding. The help centre documents token issuance but publishes neither the\n    transport (header/query) nor the parameter name.'\n  sources:\n  - https://learn.crexi.com/listing-api-overview-crexi-help-center\n  gated: true\nobservations:\n- The\
  \ OAuth 2.0 authorization server metadata document is byte-identical to the OpenID\n  Connect discovery document.\n- No authorization_endpoint is advertised — only a token endpoint — consistent with\n  the advertised grant set (resource-owner password, refresh, user switching, single-use\n  token exchange) rather than a redirect-based authorization code flow.\n- require_pushed_authorization_requests is false; tls_client_certificate_bound_access_tokens\n  is false; authorization_response_iss_parameter_supported is true.\n- No mutualTLS scheme and no PKCE/authorization-code metadata are published.\nx-evidence:\n  fetched: '2026-08-01'\n  urls:\n  - url: https://api.crexi.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://api.crexi.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://api.crexi.com/swagger/v1/swagger.json\n    http_status: 401\n  - url: https://exchange.crexi.com/Content/auth.js\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crexi/refs/heads/main/authentication/crexi-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 5 schemes
tags:
- Real Estate
- Commercial Real Estate
- Marketplace
- Property Data
- Listings
- Auctions
- Market Intelligence
- Data Syndication
- RESO
- Company
---
