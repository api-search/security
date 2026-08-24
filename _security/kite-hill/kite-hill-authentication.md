---
api_key_in: []
auth_types:
- none
- openIdConnect
- oauth2
- agentProfile
- http
description: Kite Hill publishes no OpenAPI, so this profile is built from live discovery documents and observed responses rather than derived securitySchemes. Five distinct auth postures were observed on 2026-08-23 — and notably, THREE of the machine surfaces answered with no credential at all.
kind: authentication
layout: security
method: probed
name: Kite Hill Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Kite Hill secures its APIs with none, openIdConnect, oauth2, agentProfile, and http across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Kite Hill
provider_slug: kite-hill
scheme_count: 7
schemes:
- name: anonymous-storefront-graphql
  observed: Full GraphQL introspection succeeded with no X-Shopify-Storefront-Access-Token header, on five separate API versions (2026-04, 2026-01, 2025-07, 2025-01, unstable). Cost limiting is signalled via extensions.cost on every response rather than by an auth challenge.
  sources:
  - graphql/kite-hill-graphql.yml
  surface: https://kite-hill.com/api/2026-04/graphql.json
  type: none
- name: anonymous-storefront-mcp
  observed: An unauthenticated JSON-RPC tools/list returned HTTP 200 with five tools and their input schemas. No Authorization header, API key or Storefront token required.
  sources:
  - mcp/kite-hill-mcp.yml
  surface: https://kite-hill.com/api/mcp
  type: none
- name: anonymous-ucp-mcp-discovery
  observed: An unauthenticated tools/list returned HTTP 200 with all thirteen commerce tools, including complete_checkout. Discovery of the commerce surface requires no credential.
  sources:
  - mcp/kite-hill-mcp.yml
  surface: https://kite-hill.com/api/ucp/mcp
  type: none
- mechanism: 'Every one of the thirteen UCP tools declares meta["ucp-agent"]["profile"] — a resolvable agent profile URI — as a REQUIRED input property. resources/list and prompts/list already fail without it, returning HTTP 422 and JSON-RPC error -32001 "UCP discovery failed" with code invalid_profile_url ("Unable to fetch agent profile: Missing profile uri").'
  name: ucp-agent-profile
  note: This is agent IDENTITY, not shopper authorization. Payment authorization is separate and, per the provider's own robots.txt, must be approved by a human at the time of purchase.
  observed: 'Confirmed 2026-08-23: tools/list is open, but the agent-identity requirement is enforced on invocation and on the resource/prompt methods.'
  sources:
  - mcp/kite-hill-ucp-mcp-tools.json
  - well-known/kite-hill-ucp.json
  spec: https://ucp.dev/2026-04-08/specification/overview/
  surface: https://kite-hill.com/api/ucp/mcp
  type: agentProfile
- authorizationUrl: https://shopify.com/authentication/68089118898/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/68089118898/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/68089118898
  jwks_uri: https://shopify.com/authentication/68089118898/.well-known/jwks.json
  name: shopify-customer-accounts
  openIdConnectUrl: https://kite-hill.com/.well-known/openid-configuration
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
  - well-known/kite-hill-openid-configuration.json
  tokenUrl: https://shopify.com/authentication/68089118898/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
- name: shopify-customer-accounts-oauth2
  note: The same authorization server also publishes RFC 8414 metadata at /.well-known/oauth-authorization-server (byte-identical document), so the surface is usable as plain OAuth 2.0 as well as OIDC.
  sources:
  - well-known/kite-hill-oauth-authorization-server.json
  type: oauth2
- header: X-Shopify-Customer-Access-Token
  mechanism: The Storefront GraphQL schema itself carries a legacy shopper-token flow — customerAccessTokenCreate / customerAccessTokenRenew / customerAccessTokenDelete / customerAccessTokenCreateWithMultipass mutations, consumed by the customer query and the customer* mutations. Distinct from the OIDC customer-accounts flow above.
  name: storefront-customer-access-token
  scheme: bearer
  sources:
  - graphql/kite-hill-storefront.graphql
  surface: https://kite-hill.com/api/2026-04/graphql.json
  type: http
slug: kite-hill-authentication
source_filename: kite-hill-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://kite-hill.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\ndescription: >-\n  Kite Hill publishes no OpenAPI, so this profile is built from live discovery documents and\n  observed responses rather than derived securitySchemes. Five distinct auth postures were\n  observed on 2026-08-23 — and notably, THREE of the machine surfaces answered with no\n  credential at all.\nsummary:\n  types: [none, openIdConnect, oauth2, agentProfile, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\nschemes:\n- name: anonymous-storefront-graphql\n  type: none\n  surface: https://kite-hill.com/api/2026-04/graphql.json\n  observed: >-\n    Full GraphQL introspection succeeded with no X-Shopify-Storefront-Access-Token header,\n    on five separate API versions (2026-04, 2026-01, 2025-07, 2025-01, unstable). Cost\n    limiting is signalled via extensions.cost on every response\
  \ rather than by an auth\n    challenge.\n  sources: [graphql/kite-hill-graphql.yml]\n- name: anonymous-storefront-mcp\n  type: none\n  surface: https://kite-hill.com/api/mcp\n  observed: >-\n    An unauthenticated JSON-RPC tools/list returned HTTP 200 with five tools and their input\n    schemas. No Authorization header, API key or Storefront token required.\n  sources: [mcp/kite-hill-mcp.yml]\n- name: anonymous-ucp-mcp-discovery\n  type: none\n  surface: https://kite-hill.com/api/ucp/mcp\n  observed: >-\n    An unauthenticated tools/list returned HTTP 200 with all thirteen commerce tools,\n    including complete_checkout. Discovery of the commerce surface requires no credential.\n  sources: [mcp/kite-hill-mcp.yml]\n- name: ucp-agent-profile\n  type: agentProfile\n  surface: https://kite-hill.com/api/ucp/mcp\n  mechanism: >-\n    Every one of the thirteen UCP tools declares meta[\"ucp-agent\"][\"profile\"] — a resolvable\n    agent profile URI — as a REQUIRED input property. resources/list\
  \ and prompts/list\n    already fail without it, returning HTTP 422 and JSON-RPC error -32001 \"UCP discovery\n    failed\" with code invalid_profile_url (\"Unable to fetch agent profile: Missing profile\n    uri\").\n  observed: >-\n    Confirmed 2026-08-23: tools/list is open, but the agent-identity requirement is enforced\n    on invocation and on the resource/prompt methods.\n  spec: https://ucp.dev/2026-04-08/specification/overview/\n  note: >-\n    This is agent IDENTITY, not shopper authorization. Payment authorization is separate and,\n    per the provider's own robots.txt, must be approved by a human at the time of purchase.\n  sources: [mcp/kite-hill-ucp-mcp-tools.json, well-known/kite-hill-ucp.json]\n- name: shopify-customer-accounts\n  type: openIdConnect\n  openIdConnectUrl: https://kite-hill.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/68089118898\n  authorizationUrl: https://shopify.com/authentication/68089118898/oauth/authorize\n  tokenUrl:\
  \ https://shopify.com/authentication/68089118898/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/68089118898/logout\n  jwks_uri: https://shopify.com/authentication/68089118898/.well-known/jwks.json\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  pkce: [S256]\n  id_token_signing_alg: [RS256]\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  sources: [well-known/kite-hill-openid-configuration.json]\n- name: shopify-customer-accounts-oauth2\n  type: oauth2\n  note: >-\n    The same authorization server also publishes RFC 8414 metadata at\n    /.well-known/oauth-authorization-server (byte-identical document), so the surface is\n    usable as plain OAuth 2.0 as well as OIDC.\n  sources: [well-known/kite-hill-oauth-authorization-server.json]\n\
  - name: storefront-customer-access-token\n  type: http\n  scheme: bearer\n  surface: https://kite-hill.com/api/2026-04/graphql.json\n  header: X-Shopify-Customer-Access-Token\n  mechanism: >-\n    The Storefront GraphQL schema itself carries a legacy shopper-token flow —\n    customerAccessTokenCreate / customerAccessTokenRenew / customerAccessTokenDelete /\n    customerAccessTokenCreateWithMultipass mutations, consumed by the customer query and the\n    customer* mutations. Distinct from the OIDC customer-accounts flow above.\n  sources: [graphql/kite-hill-storefront.graphql]\nhuman_web:\n  login: https://kite-hill.com/account/login\n  register: https://kite-hill.com/account/register\n  observed: >-\n    Both 302 to https://shopify.com/68089118898/account — Shopify's hosted new customer\n    accounts, i.e. the OIDC surface above rather than a store-local password form.\nx-evidence:\n- fetched: '2026-08-23'\n  url: https://kite-hill.com/.well-known/openid-configuration\n  http_status:\
  \ 200\n- fetched: '2026-08-23'\n  url: https://kite-hill.com/api/2026-04/graphql.json\n  http_status: 200\n  note: anonymous introspection\n- fetched: '2026-08-23'\n  url: https://kite-hill.com/api/ucp/mcp\n  http_status: 200\n  note: anonymous tools/list; resources/list rejected 422 with -32001 invalid_profile_url\n- fetched: '2026-08-23'\n  url: https://kite-hill.com/account/login\n  http_status: 302\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kite-hill/refs/heads/main/authentication/kite-hill-authentication.yml
summary_line: none/openIdConnect/oauth2/agentProfile/http · 7 schemes
tags:
- Company
- Consumer Packaged Goods
- Plant Based Foods
- Dairy Alternatives
- Food and Beverage
- E-Commerce
- Direct to Consumer
- Retail
- Agentic Commerce
- Shopify
- GraphQL
- MCP
- Universal Commerce Protocol
---
