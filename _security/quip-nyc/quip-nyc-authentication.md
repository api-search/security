---
api_key_in:
- header
auth_types:
- none
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: probed
name: Quip Nyc Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Quip NYC secures its APIs with none, oauth2, openIdConnect, and apiKey across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Quip NYC
provider_slug: quip-nyc
scheme_count: 7
schemes:
- applies_to: https://www.getquip.com/api/ucp/mcp
  name: anonymous-ucp-mcp-discovery
  observed: initialize and tools/list both returned HTTP 200 with the full 13-tool set and complete JSON Schema input schemas, with no credential of any kind.
  type: none
- applies_to: https://www.getquip.com/api/ucp/mcp
  in: body
  name: ucp-agent-profile
  note: Recorded as apiKey/in:body because no standard scheme type describes it. It is the UCP agent-identity mechanism, and it is the only mandatory field on all thirteen tools.
  observed: 'Every tools/call — and prompts/list and resources/list — returns HTTP 422 with JSON-RPC error -32001 "UCP discovery failed" (data.code invalid_profile_url, "Missing profile uri") unless a resolvable agent profile URI is supplied. This is an identity control, not a secret: the value is a public URI the agent publishes about itself, not a bearer token.'
  parameter: meta.ucp-agent.profile
  required: true
  type: apiKey
- applies_to: https://www.getquip.com/api/2026-07/graphql.json
  name: anonymous-storefront-graphql
  note: Customer-scoped fields still require a customerAccessToken obtained via the customerAccessTokenCreate mutation.
  observed: Full introspection returned HTTP 200 (415 types, 34 query root fields, 41 mutations) with no X-Shopify-Storefront-Access-Token header.
  type: none
- applies_to: https://www.getquip.com/
  name: anonymous-storefront-json
  observed: /products.json?limit=3 and /collections/all/products.json?limit=2 both returned HTTP 200 unauthenticated with real product records.
  type: none
- applies_to: Customer account sign-in at https://www.getquip.com/account/login
  authorizationUrl: https://shopify.com/authentication/57677807690/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/57677807690/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/57677807690
  jwks_uri: https://shopify.com/authentication/57677807690/.well-known/jwks.json
  name: shopify-customer-accounts-oidc
  openIdConnectUrl: https://www.getquip.com/.well-known/openid-configuration
  pkce:
  - S256
  provider: Shopify Customer Accounts (shop id 57677807690)
  response_types:
  - code
  subject_types:
  - public
  tokenUrl: https://shopify.com/authentication/57677807690/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
- flows:
  - authorizationUrl: https://shopify.com/authentication/57677807690/oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://shopify.com/authentication/57677807690/oauth/token
  name: shopify-customer-account-oauth2
  note: The RFC 8414 metadata document is byte-identical to the OIDC discovery document.
  source: https://www.getquip.com/.well-known/oauth-authorization-server
  type: oauth2
- applies_to: https://www.getquip.com/api/2026-07/graphql.json
  in: header
  name: customer-access-token
  note: Documented by the platform vendor, not by quip.
  observed: Required by the customer query field per the introspected schema; obtained via customerAccessTokenCreate.
  parameter: X-Shopify-Customer-Access-Token
  type: apiKey
slug: quip-nyc-authentication
source_filename: quip-nyc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource:\n- https://www.getquip.com/.well-known/openid-configuration\n- https://www.getquip.com/.well-known/oauth-authorization-server\n- https://www.getquip.com/.well-known/oauth-protected-resource\n- https://www.getquip.com/api/ucp/mcp\n- https://www.getquip.com/api/2026-07/graphql.json\ndocs: https://www.getquip.com/agents.md\nnote: >-\n  Derived from live probes, not from an OpenAPI document — quip publishes no spec, so\n  derive-authentication.py has no openapi/ directory to read. This file records the auth\n  model actually observed on the wire against quip's own hosts.\nsummary:\n  types: [none, oauth2, openIdConnect, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\n  anonymous_surfaces: 3\nschemes:\n- name: anonymous-ucp-mcp-discovery\n  type: none\n  applies_to: https://www.getquip.com/api/ucp/mcp\n  observed: >-\n    initialize and tools/list both returned HTTP 200 with the full\
  \ 13-tool set and complete\n    JSON Schema input schemas, with no credential of any kind.\n- name: ucp-agent-profile\n  type: apiKey\n  in: body\n  parameter: meta.ucp-agent.profile\n  applies_to: https://www.getquip.com/api/ucp/mcp\n  required: true\n  observed: >-\n    Every tools/call — and prompts/list and resources/list — returns HTTP 422 with JSON-RPC\n    error -32001 \"UCP discovery failed\" (data.code invalid_profile_url, \"Missing profile uri\")\n    unless a resolvable agent profile URI is supplied. This is an identity control, not a\n    secret: the value is a public URI the agent publishes about itself, not a bearer token.\n  note: >-\n    Recorded as apiKey/in:body because no standard scheme type describes it. It is the\n    UCP agent-identity mechanism, and it is the only mandatory field on all thirteen tools.\n- name: anonymous-storefront-graphql\n  type: none\n  applies_to: https://www.getquip.com/api/2026-07/graphql.json\n  observed: >-\n    Full introspection returned\
  \ HTTP 200 (415 types, 34 query root fields, 41 mutations)\n    with no X-Shopify-Storefront-Access-Token header.\n  note: >-\n    Customer-scoped fields still require a customerAccessToken obtained via the\n    customerAccessTokenCreate mutation.\n- name: anonymous-storefront-json\n  type: none\n  applies_to: https://www.getquip.com/\n  observed: >-\n    /products.json?limit=3 and /collections/all/products.json?limit=2 both returned HTTP 200\n    unauthenticated with real product records.\n- name: shopify-customer-accounts-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://www.getquip.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/57677807690\n  authorizationUrl: https://shopify.com/authentication/57677807690/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/57677807690/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/57677807690/logout\n  jwks_uri: https://shopify.com/authentication/57677807690/.well-known/jwks.json\n\
  \  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  pkce: [S256]\n  id_token_signing_alg: [RS256]\n  subject_types: [public]\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  applies_to: Customer account sign-in at https://www.getquip.com/account/login\n  provider: Shopify Customer Accounts (shop id 57677807690)\n- name: shopify-customer-account-oauth2\n  type: oauth2\n  source: https://www.getquip.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/57677807690/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/57677807690/oauth/token\n    scopes: 4\n  note: The RFC 8414 metadata document is byte-identical to the OIDC discovery document.\n- name: customer-access-token\n  type: apiKey\n  in: header\n  parameter: X-Shopify-Customer-Access-Token\n\
  \  applies_to: https://www.getquip.com/api/2026-07/graphql.json\n  observed: >-\n    Required by the customer query field per the introspected schema; obtained via\n    customerAccessTokenCreate.\n  note: Documented by the platform vendor, not by quip.\nprotected_resource:\n  source: https://www.getquip.com/.well-known/oauth-protected-resource\n  spec: RFC 9728 OAuth 2.0 Protected Resource Metadata\n  resource: https://www.getquip.com\n  authorization_servers: ['https://shopify.com/authentication/57677807690']\n  bearer_methods_supported: [header]\nx-evidence:\n- url: https://www.getquip.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n- url: https://www.getquip.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n- url: https://www.getquip.com/.well-known/oauth-protected-resource\n  http_status: 200\n  content_type: application/json\n- url: https://www.getquip.com/api/ucp/mcp\n  http_status: 200\n\
  \  note: anonymous initialize + tools/list\n- url: https://www.getquip.com/api/ucp/mcp\n  http_status: 422\n  note: tools/call without meta.ucp-agent.profile\n- url: https://www.getquip.com/api/2026-07/graphql.json\n  http_status: 200\n  note: anonymous full introspection\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quip-nyc/refs/heads/main/authentication/quip-nyc-authentication.yml
summary_line: none/oauth2/openIdConnect/apiKey · 7 schemes
tags:
- Company
- Oral Care
- Consumer Health
- Personal Care
- Retail
- E-Commerce
- Direct to Consumer
- Subscription
- Agentic Commerce
- Shopify
---
