---
api_key_in: []
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Premier Lacrosse League Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- urn:ietf:params:oauth:grant-type:jwt-bearer
overview: Premier Lacrosse League secures its APIs with none, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and urn:ietf:params:oauth:grant-type:jwt-bearer flow(s).
provider_name: Premier Lacrosse League
provider_slug: premier-lacrosse-league
scheme_count: 4
schemes:
- applies_to: https://premierlacrosseleague.com/api/graphql
  description: The Apollo Server GraphQL API that backs the league's web and stats properties requires no credential, but enforces a CORS-style origin allow-list at the application layer. A POST without an allowed Origin header returns HTTP 403 with body {"error":"Origin not allowed"}. With Origin set to https://premierlacrosseleague.com the request is accepted and validated. There is no published way for a third party to obtain authorized access.
  introspection_disabled: true
  name: web-graphql-origin-restricted
  observed:
    allowed_origin:
      http_status: 400
      note: request accepted, failed GraphQL validation only
    no_origin:
      body: '{"error":"Origin not allowed"}'
      http_status: 403
  type: none
- applies_to: https://shop.premierlacrosseleague.com
  description: Product and collection JSON on the store is served unauthenticated (GET /products/{handle}.json, GET /collections/{handle}/products.json, GET /search?q={query}&type=product). Documented by the store's own llms.txt.
  name: shop-storefront-public-json
  observed:
    example:
      content_type: application/json
      http_status: 200
      url: https://shop.premierlacrosseleague.com/collections/all/products.json?limit=2
  type: none
- applies_to: https://shop.premierlacrosseleague.com
  authorizationUrl: https://account.premierlacrosseleague.com/authentication/oauth/authorize
  description: OAuth 2.0 / OpenID Connect authorization server for shop customer accounts, discovered via RFC 8414 and OIDC Discovery. Backs both the customer account API and the authenticated customer-account MCP API used for agent commerce.
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/8037761076
  jwksUri: https://account.premierlacrosseleague.com/authentication/.well-known/jwks.json
  name: shop-customer-accounts
  pkce:
  - S256
  scopes: 4
  scopes_file: scopes/premier-lacrosse-league-scopes.yml
  sources:
  - well-known/premier-lacrosse-league-shop-oauth-authorization-server.json
  - well-known/premier-lacrosse-league-shop-oauth-protected-resource.json
  subtype: openIdConnect
  tokenUrl: https://account.premierlacrosseleague.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: oauth2
- applies_to: https://shop.premierlacrosseleague.com/api/ucp/mcp
  bearer_methods_supported:
  - header
  description: 'The store''s MCP endpoint does not gate on a bearer token for tools/list; it gates on a UCP agent profile URI. An anonymous tools/list returns HTTP 422 with JSON-RPC error -32001 invalid_profile_url ("Unable to fetch agent profile: Missing profile uri"). Payment completion additionally requires contemporaneous human buyer approval.'
  name: shop-ucp-agent-profile
  type: agent-identity
slug: premier-lacrosse-league-authentication
source_filename: premier-lacrosse-league-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: >-\n  live probes of premierlacrosseleague.com/api/graphql, shop.premierlacrosseleague.com and its\n  /.well-known/ discovery documents on 2026-08-02\ndocs: null\nnote: >-\n  Derived from probes, not from an OpenAPI document — the Premier Lacrosse League publishes no\n  OpenAPI, no developer portal and no authentication documentation. Nothing here is inferred; each\n  scheme records an observed response.\nsummary:\n  types: [none, oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  public_read_surfaces: 2\n  developer_credentials_available: false\nschemes:\n- name: web-graphql-origin-restricted\n  type: none\n  applies_to: https://premierlacrosseleague.com/api/graphql\n  description: >-\n    The Apollo Server GraphQL API that backs the league's web and stats properties requires no\n    credential, but enforces a CORS-style origin allow-list\
  \ at the application layer. A POST\n    without an allowed Origin header returns HTTP 403 with body {\"error\":\"Origin not allowed\"}.\n    With Origin set to https://premierlacrosseleague.com the request is accepted and validated.\n    There is no published way for a third party to obtain authorized access.\n  observed:\n    no_origin: {http_status: 403, body: '{\"error\":\"Origin not allowed\"}'}\n    allowed_origin: {http_status: 400, note: 'request accepted, failed GraphQL validation only'}\n  introspection_disabled: true\n- name: shop-storefront-public-json\n  type: none\n  applies_to: https://shop.premierlacrosseleague.com\n  description: >-\n    Product and collection JSON on the store is served unauthenticated\n    (GET /products/{handle}.json, GET /collections/{handle}/products.json,\n    GET /search?q={query}&type=product). Documented by the store's own llms.txt.\n  observed:\n    example: {url: 'https://shop.premierlacrosseleague.com/collections/all/products.json?limit=2',\
  \ http_status: 200, content_type: application/json}\n- name: shop-customer-accounts\n  type: oauth2\n  subtype: openIdConnect\n  applies_to: https://shop.premierlacrosseleague.com\n  description: >-\n    OAuth 2.0 / OpenID Connect authorization server for shop customer accounts, discovered via\n    RFC 8414 and OIDC Discovery. Backs both the customer account API and the authenticated\n    customer-account MCP API used for agent commerce.\n  issuer: https://shopify.com/authentication/8037761076\n  authorizationUrl: https://account.premierlacrosseleague.com/authentication/oauth/authorize\n  tokenUrl: https://account.premierlacrosseleague.com/authentication/oauth/token\n  jwksUri: https://account.premierlacrosseleague.com/authentication/.well-known/jwks.json\n  pkce: [S256]\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  scopes: 4\n  scopes_file: scopes/premier-lacrosse-league-scopes.yml\n  sources:\n  - well-known/premier-lacrosse-league-shop-oauth-authorization-server.json\n\
  \  - well-known/premier-lacrosse-league-shop-oauth-protected-resource.json\n- name: shop-ucp-agent-profile\n  type: agent-identity\n  applies_to: https://shop.premierlacrosseleague.com/api/ucp/mcp\n  description: >-\n    The store's MCP endpoint does not gate on a bearer token for tools/list; it gates on a UCP\n    agent profile URI. An anonymous tools/list returns HTTP 422 with JSON-RPC error -32001\n    invalid_profile_url (\"Unable to fetch agent profile: Missing profile uri\"). Payment completion\n    additionally requires contemporaneous human buyer approval.\n  bearer_methods_supported: [header]\ngaps:\n- No API key programme, no developer registration, no partner/media data-access documentation.\n- No security.txt on any host, so no published security contact.\nx-evidence:\n  fetched: '2026-08-02'\n  probes:\n  - {url: 'https://premierlacrosseleague.com/api/graphql', method: POST, http_status: 403, note: no Origin header}\n  - {url: 'https://premierlacrosseleague.com/api/graphql',\
  \ method: POST, http_status: 400, note: with allowed Origin; INTROSPECTION_DISABLED}\n  - {url: 'https://shop.premierlacrosseleague.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://shop.premierlacrosseleague.com/.well-known/oauth-protected-resource', http_status: 200}\n  - {url: 'https://shop.premierlacrosseleague.com/api/ucp/mcp', method: POST, http_status: 422}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/premier-lacrosse-league/refs/heads/main/authentication/premier-lacrosse-league-authentication.yml
summary_line: none/oauth2/openIdConnect · 4 schemes
tags:
- Company
- Sports
- Lacrosse
- Professional Sports League
- Sports Statistics
- Media and Entertainment
- E-Commerce
- Agent Commerce
- GraphQL
- Fantasy Sports
---
