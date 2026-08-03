---
api_key_in: []
auth_types:
- none
- openIdConnect
- oauth2
description: Bobbie publishes no OpenAPI, so this profile is built from live discovery documents and observed responses rather than derived securitySchemes. Three distinct auth postures were observed on 2026-08-02.
kind: authentication
layout: security
method: probed
name: Bobbie Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Bobbie secures its APIs with none, openIdConnect, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Bobbie
provider_slug: bobbie
scheme_count: 5
schemes:
- name: anonymous-storefront-mcp
  observed: An unauthenticated JSON-RPC tools/list returned HTTP 200 with the full tool set and input schemas. No Authorization header, API key or Storefront token required.
  sources:
  - mcp/bobbie-mcp.yml
  surface: https://www.hibobbie.com/api/mcp
  type: none
- name: anonymous-storefront-graphql
  observed: Full GraphQL introspection succeeded with no X-Shopify-Storefront-Access-Token header. Rate/cost limiting is signalled via extensions.cost on every response.
  sources:
  - graphql/bobbie-graphql.yml
  surface: https://www.hibobbie.com/api/2026-04/graphql.json
  type: none
- authorizationUrl: https://account.hibobbie.com/authentication/oauth/authorize
  claims:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  end_session_endpoint: https://account.hibobbie.com/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/6622806101
  jwks_uri: https://account.hibobbie.com/authentication/.well-known/jwks.json
  name: shopify-customer-accounts
  openIdConnectUrl: https://www.hibobbie.com/.well-known/openid-configuration
  pkce:
  - S256
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/bobbie-openid-configuration.json
  tokenUrl: https://account.hibobbie.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- name: shopify-customer-accounts-oauth2
  note: The same authorization server also publishes RFC 8414 metadata at /.well-known/oauth-authorization-server (byte-identical document), so the surface is usable as plain OAuth 2.0 as well as OIDC.
  sources:
  - well-known/bobbie-oauth-authorization-server.json
  type: oauth2
- name: ucp-agent-profile
  observed: tools/list without an agent profile URI returns JSON-RPC -32001 "UCP discovery failed" / invalid_profile_url. The UCP commerce surface therefore requires an agent to present a resolvable profile before any tool call, and checkout completion additionally requires contemporaneous buyer approval (see agentic-access/).
  sources:
  - well-known/bobbie-ucp.json
  - llms/bobbie-llms.txt
  spec: https://ucp.dev/2026-04-08/specification/overview/
  surface: https://www.hibobbie.com/api/ucp/mcp
  type: other
slug: bobbie-authentication
source_filename: bobbie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://www.hibobbie.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\ndescription: >-\n  Bobbie publishes no OpenAPI, so this profile is built from live discovery documents\n  and observed responses rather than derived securitySchemes. Three distinct auth\n  postures were observed on 2026-08-02.\nsummary:\n  types: [none, openIdConnect, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\nschemes:\n  - name: anonymous-storefront-mcp\n    type: none\n    surface: https://www.hibobbie.com/api/mcp\n    observed: >-\n      An unauthenticated JSON-RPC tools/list returned HTTP 200 with the full tool set\n      and input schemas. No Authorization header, API key or Storefront token required.\n    sources: [mcp/bobbie-mcp.yml]\n  - name: anonymous-storefront-graphql\n    type: none\n    surface: https://www.hibobbie.com/api/2026-04/graphql.json\n    observed: >-\n\
  \      Full GraphQL introspection succeeded with no X-Shopify-Storefront-Access-Token\n      header. Rate/cost limiting is signalled via extensions.cost on every response.\n    sources: [graphql/bobbie-graphql.yml]\n  - name: shopify-customer-accounts\n    type: openIdConnect\n    openIdConnectUrl: https://www.hibobbie.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/6622806101\n    authorizationUrl: https://account.hibobbie.com/authentication/oauth/authorize\n    tokenUrl: https://account.hibobbie.com/authentication/oauth/token\n    end_session_endpoint: https://account.hibobbie.com/authentication/logout\n    jwks_uri: https://account.hibobbie.com/authentication/.well-known/jwks.json\n    grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    response_types: [code]\n    token_endpoint_auth_methods: [client_secret_basic]\n    pkce: [S256]\n    id_token_signing_alg: [RS256]\n    claims: [iss, sub, aud, exp,\
  \ iat, nonce, sid, email, email_verified]\n    scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n    sources: [well-known/bobbie-openid-configuration.json]\n  - name: shopify-customer-accounts-oauth2\n    type: oauth2\n    note: >-\n      The same authorization server also publishes RFC 8414 metadata at\n      /.well-known/oauth-authorization-server (byte-identical document), so the surface\n      is usable as plain OAuth 2.0 as well as OIDC.\n    sources: [well-known/bobbie-oauth-authorization-server.json]\n  - name: ucp-agent-profile\n    type: other\n    surface: https://www.hibobbie.com/api/ucp/mcp\n    observed: >-\n      tools/list without an agent profile URI returns JSON-RPC -32001\n      \"UCP discovery failed\" / invalid_profile_url. The UCP commerce surface therefore\n      requires an agent to present a resolvable profile before any tool call, and\n      checkout completion additionally requires contemporaneous buyer approval\n      (see\
  \ agentic-access/).\n    spec: https://ucp.dev/2026-04-08/specification/overview/\n    sources: [well-known/bobbie-ucp.json, llms/bobbie-llms.txt]\nplatform:\n  vendor: Shopify\n  note: >-\n    The identity provider is Shopify's, bound to Bobbie's shop id 6622806101 and served\n    from Bobbie's account.hibobbie.com vanity domain.\nx-evidence:\n  - fetched: '2026-08-02'\n    url: https://www.hibobbie.com/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json\n  - fetched: '2026-08-02'\n    url: https://www.hibobbie.com/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bobbie/refs/heads/main/authentication/bobbie-authentication.yml
summary_line: none/openIdConnect/oauth2 · 5 schemes
tags:
- Company
- Consumer Packaged Goods
- Infant Formula
- Ecommerce
- Direct to Consumer
- Retail
- Health
- Nutrition
- Agentic Commerce
- Shopify
- GraphQL
- Model Context Protocol
---
