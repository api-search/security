---
api_key_in: []
auth_types:
- none
- openIdConnect
- oauth2
- other
description: Fnatic publishes no OpenAPI, so this profile is built from live discovery documents and observed responses rather than derived securitySchemes. Four distinct auth postures were observed across Fnatic hosts on 2026-08-04. Note that fnatic.com's own member accounts (Fnatic ID) are a first-party login surface with NO published discovery document — only the Shopify-hosted shop exposes machine-readable identity metadata.
kind: authentication
layout: security
method: probed
name: Fnatic Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Fnatic secures its APIs with none, openIdConnect, oauth2, and other across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Fnatic
provider_slug: fnatic
scheme_count: 5
schemes:
- name: anonymous-storefront-graphql
  observed: Full GraphQL introspection succeeded with no X-Shopify-Storefront-Access-Token header (HTTP 200, 755,648 bytes). Cost/rate limiting is signalled via extensions.cost on every response rather than by rejecting anonymous callers.
  sources:
  - graphql/fnatic-graphql.yml
  surface: https://shop.fnatic.com/api/2026-04/graphql.json
  type: none
- authorizationUrl: https://shopify.com/authentication/54359195821/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/54359195821/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/54359195821
  jwks_uri: https://shopify.com/authentication/54359195821/.well-known/jwks.json
  name: shopify-customer-accounts
  openIdConnectUrl: https://shop.fnatic.com/.well-known/openid-configuration
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
  - well-known/fnatic-openid-configuration.json
  tokenUrl: https://shopify.com/authentication/54359195821/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- authorization_servers:
  - https://shopify.com/authentication/54359195821
  bearer_methods_supported:
  - header
  name: shopify-customer-accounts-oauth2
  note: The same authorization server also publishes RFC 8414 metadata at /.well-known/oauth-authorization-server (byte-identical document), and an RFC 9728 protected-resource document at /.well-known/oauth-protected-resource declaring resource https://shop.fnatic.com with bearer_methods_supported [header]. The surface is therefore usable as plain OAuth 2.0 as well as OIDC.
  resource: https://shop.fnatic.com
  sources:
  - well-known/fnatic-oauth-authorization-server.json
  - well-known/fnatic-oauth-protected-resource.json
  type: oauth2
- name: storefront-customer-access-token
  observed: 'The legacy Storefront customer surface issues an opaque CustomerAccessToken via Mutation.customerAccessTokenCreate(input: CustomerAccessTokenCreateInput) and it is passed to QueryRoot.customer(customerAccessToken:) and every customer* mutation. Renewed with customerAccessTokenRenew, revoked with customerAccessTokenDelete. Multipass SSO is also present (customerAccessTokenCreateWithMultipass).'
  sources:
  - graphql/fnatic-storefront.graphql
  surface: https://shop.fnatic.com/api/2026-04/graphql.json
  type: other
- name: ucp-agent-profile
  observed: tools/list without an agent profile URI returns HTTP 422 with JSON-RPC -32001 "UCP discovery failed" / invalid_profile_url. The UCP commerce surface therefore requires an agent to present a resolvable profile before any tool call, and Fnatic additionally requires contemporaneous buyer approval before complete_checkout.
  sources:
  - well-known/fnatic-ucp.json
  - llms/fnatic-agents.md
  spec: https://ucp.dev/2026-04-08/specification/overview/
  surface: https://shop.fnatic.com/api/ucp/mcp
  type: other
slug: fnatic-authentication
source_filename: fnatic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://shop.fnatic.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\ndescription: >-\n  Fnatic publishes no OpenAPI, so this profile is built from live discovery documents and\n  observed responses rather than derived securitySchemes. Four distinct auth postures\n  were observed across Fnatic hosts on 2026-08-04. Note that fnatic.com's own member\n  accounts (Fnatic ID) are a first-party login surface with NO published discovery\n  document — only the Shopify-hosted shop exposes machine-readable identity metadata.\nsummary:\n  types: [none, openIdConnect, oauth2, other]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\nschemes:\n  - name: anonymous-storefront-graphql\n    type: none\n    surface: https://shop.fnatic.com/api/2026-04/graphql.json\n    observed: >-\n      Full GraphQL introspection succeeded with no X-Shopify-Storefront-Access-Token\n      header\
  \ (HTTP 200, 755,648 bytes). Cost/rate limiting is signalled via\n      extensions.cost on every response rather than by rejecting anonymous callers.\n    sources: [graphql/fnatic-graphql.yml]\n  - name: shopify-customer-accounts\n    type: openIdConnect\n    openIdConnectUrl: https://shop.fnatic.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/54359195821\n    authorizationUrl: https://shopify.com/authentication/54359195821/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/54359195821/oauth/token\n    end_session_endpoint: https://shopify.com/authentication/54359195821/logout\n    jwks_uri: https://shopify.com/authentication/54359195821/.well-known/jwks.json\n    grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    response_types: [code]\n    token_endpoint_auth_methods: [client_secret_basic]\n    pkce: [S256]\n    id_token_signing_alg: [RS256]\n    claims: [iss, sub, aud, exp, iat, nonce,\
  \ sid, email, email_verified]\n    scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n    sources: [well-known/fnatic-openid-configuration.json]\n  - name: shopify-customer-accounts-oauth2\n    type: oauth2\n    note: >-\n      The same authorization server also publishes RFC 8414 metadata at\n      /.well-known/oauth-authorization-server (byte-identical document), and an RFC 9728\n      protected-resource document at /.well-known/oauth-protected-resource declaring\n      resource https://shop.fnatic.com with bearer_methods_supported [header]. The\n      surface is therefore usable as plain OAuth 2.0 as well as OIDC.\n    resource: https://shop.fnatic.com\n    authorization_servers: ['https://shopify.com/authentication/54359195821']\n    bearer_methods_supported: [header]\n    sources:\n      - well-known/fnatic-oauth-authorization-server.json\n      - well-known/fnatic-oauth-protected-resource.json\n  - name: storefront-customer-access-token\n    type:\
  \ other\n    surface: https://shop.fnatic.com/api/2026-04/graphql.json\n    observed: >-\n      The legacy Storefront customer surface issues an opaque CustomerAccessToken via\n      Mutation.customerAccessTokenCreate(input: CustomerAccessTokenCreateInput) and it is\n      passed to QueryRoot.customer(customerAccessToken:) and every customer* mutation.\n      Renewed with customerAccessTokenRenew, revoked with customerAccessTokenDelete.\n      Multipass SSO is also present (customerAccessTokenCreateWithMultipass).\n    sources: [graphql/fnatic-storefront.graphql]\n  - name: ucp-agent-profile\n    type: other\n    surface: https://shop.fnatic.com/api/ucp/mcp\n    observed: >-\n      tools/list without an agent profile URI returns HTTP 422 with JSON-RPC -32001\n      \"UCP discovery failed\" / invalid_profile_url. The UCP commerce surface therefore\n      requires an agent to present a resolvable profile before any tool call, and Fnatic\n      additionally requires contemporaneous buyer\
  \ approval before complete_checkout.\n    spec: https://ucp.dev/2026-04-08/specification/overview/\n    sources: [well-known/fnatic-ucp.json, llms/fnatic-agents.md]\nnot_public:\n  - name: fnatic-id\n    surface: https://fnatic.com/account/login\n    note: >-\n      Fnatic's own member accounts (\"Fnatic ID\") on fnatic.com — register, login,\n      change-password, connections, membership, wallet-connect. No OIDC/OAuth discovery\n      document, no documented token endpoint, no developer program. Not a machine-readable\n      auth surface.\n  - name: id.fnatic.com\n    surface: https://id.fnatic.com/\n    note: >-\n      Internal admin/identity application. Every request redirects to Google Workspace\n      sign-in restricted to hd=fnatic.com (client_id 259306135017-…apps.googleusercontent.com,\n      redirect_uri https://id.fnatic.com/nova/login-complete, scope \"openid profile email\").\n      Staff-only; recorded for completeness, not an integrable surface.\nplatform:\n  vendor: Shopify\n\
  \  note: >-\n    The identity provider is Shopify's, bound to Fnatic shop id 54359195821 and served\n    from Fnatic's shop.fnatic.com domain. Unlike some Shopify merchants, Fnatic does not\n    front the authorization endpoints on a fnatic.com vanity host — they resolve to\n    shopify.com.\nx-evidence:\n  - fetched: '2026-08-04'\n    url: https://shop.fnatic.com/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json\n  - fetched: '2026-08-04'\n    url: https://shop.fnatic.com/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json\n  - fetched: '2026-08-04'\n    url: https://shop.fnatic.com/.well-known/oauth-protected-resource\n    http_status: 200\n    content_type: application/json\n  - fetched: '2026-08-04'\n    url: https://shop.fnatic.com/api/2026-04/graphql.json\n    http_status: 200\n    result: anonymous introspection succeeded\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fnatic/refs/heads/main/authentication/fnatic-authentication.yml
summary_line: none/openIdConnect/oauth2/other · 5 schemes
tags:
- Company
- Esports
- Gaming
- Entertainment
- Sports
- Consumer Electronics
- Gaming Hardware
- Apparel
- Ecommerce
- Direct to Consumer
- Agentic Commerce
- Shopify
- GraphQL
- Universal Commerce Protocol
- Model Context Protocol
- United Kingdom
---
