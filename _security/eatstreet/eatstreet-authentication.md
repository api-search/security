---
api_key_in: []
auth_types: []
description: 'EatStreet publishes an RFC 8414 OAuth 2.0 Authorization Server Metadata document at https://eatstreet.com/.well-known/oauth-authorization-server. It is the only machine-readable contract EatStreet currently serves: the public developer portal at developers.eatstreet.com returns 404 and no OpenAPI, GraphQL SDL or MCP manifest was found on any host. Everything below is read verbatim from that metadata document and from live unauthenticated responses from the token endpoint — nothing here is inferred from documentation, because EatStreet publishes none.'
kind: authentication
layout: security
method: probed
name: Eatstreet Authentication
name_suffix: Authentication
oauth_flows: []
overview: EatStreet declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: EatStreet
provider_slug: eatstreet
scheme_count: 1
schemes:
- authorization_endpoint: https://eatstreet.com/authorize
  client_authentication:
    introspection_endpoint:
    - client_secret_basic
    - client_secret_post
    revocation_endpoint:
    - client_secret_basic
    - client_secret_post
    token_endpoint:
    - client_secret_basic
    - client_secret_post
  flow: authorization_code
  grant_types_supported:
  - authorization_code
  id: oauth2_authorization_code
  introspection_endpoint: https://eatstreet.com/api/v2/oauth/introspect
  issuer: https://eatstreet.com
  jwks_uri: https://eatstreet.com/.well-known/jwks.json
  pkce:
    code_challenge_methods:
    - plain
    - S256
    supported: true
  response_modes_supported:
  - query
  response_types_supported:
  - code
  - token
  revocation_endpoint: https://eatstreet.com/api/v2/oauth/revoke
  scopes:
  - merchant_integration
  - customer
  - example
  token_endpoint: https://eatstreet.com/api/v2/oauth/token
  type: oauth2
  ui_locales_supported:
  - en-US
slug: eatstreet-authentication
source_filename: eatstreet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://eatstreet.com/.well-known/oauth-authorization-server\nname: EatStreet authentication profile\ndescription: >-\n  EatStreet publishes an RFC 8414 OAuth 2.0 Authorization Server Metadata\n  document at https://eatstreet.com/.well-known/oauth-authorization-server. It\n  is the only machine-readable contract EatStreet currently serves: the public\n  developer portal at developers.eatstreet.com returns 404 and no OpenAPI,\n  GraphQL SDL or MCP manifest was found on any host. Everything below is read\n  verbatim from that metadata document and from live unauthenticated responses\n  from the token endpoint — nothing here is inferred from documentation,\n  because EatStreet publishes none.\nschemes:\n- id: oauth2_authorization_code\n  type: oauth2\n  flow: authorization_code\n  issuer: https://eatstreet.com\n  authorization_endpoint: https://eatstreet.com/authorize\n  token_endpoint: https://eatstreet.com/api/v2/oauth/token\n\
  \  introspection_endpoint: https://eatstreet.com/api/v2/oauth/introspect\n  revocation_endpoint: https://eatstreet.com/api/v2/oauth/revoke\n  jwks_uri: https://eatstreet.com/.well-known/jwks.json\n  grant_types_supported:\n  - authorization_code\n  response_types_supported:\n  - code\n  - token\n  response_modes_supported:\n  - query\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - plain\n    - S256\n  client_authentication:\n    token_endpoint:\n    - client_secret_basic\n    - client_secret_post\n    introspection_endpoint:\n    - client_secret_basic\n    - client_secret_post\n    revocation_endpoint:\n    - client_secret_basic\n    - client_secret_post\n  scopes:\n  - merchant_integration\n  - customer\n  - example\n  ui_locales_supported:\n  - en-US\nobservations:\n- endpoint: https://eatstreet.com/api/v2/oauth/token\n  method: POST\n  request: grant_type=authorization_code (no client credentials)\n  http_status: 401\n  body: '{\"error\":\"invalid_client\",\"error_description\"\
  :\"client_id is missing\"}'\n  note: >-\n    Live, unauthenticated probe. Confirms the endpoint is active and returns\n    RFC 6749 section 5.2 error codes.\n- endpoint: https://eatstreet.com/api/v2/oauth/token\n  method: GET\n  http_status: 405\n  body: '{\"error\":{\"message\":\"This HTTP Method was rejected\",\"code\":400}}'\n- endpoint: https://eatstreet.com/authorize\n  method: GET\n  http_status: 302\n  note: Redirects (no client_id supplied).\ngaps:\n- >-\n  No OpenID Connect. /.well-known/openid-configuration returns the SPA shell, and\n  the authorization server metadata declares no id_token support or userinfo endpoint.\n- >-\n  No RFC 9728 protected-resource metadata, so an agent cannot discover which\n  resource server the tokens are for without out-of-band knowledge.\n- >-\n  No client_credentials grant is advertised, so there is no server-to-server flow\n  without a user authorization step.\n- >-\n  No public documentation of how to register a client or obtain credentials;\
  \ the\n  developer portal named by the GitHub organization (developers.eatstreet.com)\n  returns 404.\ndocs: null\nx-evidence:\n  fetched: '2026-08-12'\n  url: https://eatstreet.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json;charset=UTF-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eatstreet/refs/heads/main/authentication/eatstreet-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Food Delivery
- Restaurants
- Online Ordering
- Marketplace
- Local Commerce
- Consumer
- Point of Sale
- OAuth
---
