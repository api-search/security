---
anonymous_access: true
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
mechanism_count: 3
method: probed
name: Adrenalineshoc Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Adrenaline Shoc secures its APIs with none, oauth2, openIdConnect, and apiKey across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Adrenaline Shoc
provider_slug: adrenalineshoc
scheme_count: 6
schemes:
- applies_to: https://www.drinkaccelerator.com/api/ucp/mcp
  name: anonymous-ucp-mcp
  note: 'tools/call is not anonymous in practice - it requires meta.ucp-agent.profile to be a resolvable URI. That is an agent-identity control, not an authentication control: no secret is exchanged and no account exists. Payment additionally enforces a human buyer-approval invariant, which is a policy control.'
  observed: tools/list returned HTTP 200 with all thirteen tools and their input schemas without any credential.
  type: none
- applies_to: https://www.drinkaccelerator.com/api/2026-07/graphql.json
  name: anonymous-storefront-graphql
  note: Customer-scoped fields still require a customerAccessToken obtained via the customerAccessTokenCreate mutation.
  observed: Full introspection returned HTTP 200 (428 types) with no X-Shopify-Storefront-Access-Token header. Versions 2026-07, 2026-04, 2025-01 and 2024-04 all answer anonymously.
  type: none
- applies_to: https://www.drinkaccelerator.com/
  name: anonymous-storefront-json
  observed: /products.json and /collections/all/products.json returned HTTP 200 unauthenticated (both empty).
  type: none
- applies_to: Customer account sign-in on the Accelerator Active Energy storefront
  authorizationUrl: https://shopify.com/authentication/7133691957/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/7133691957/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/7133691957
  jwks_uri: https://shopify.com/authentication/7133691957/.well-known/jwks.json
  name: shopify-customer-accounts-oidc
  note: The discovery document is served from the company's own hosts (www.drinkaccelerator.com, drinkaccelerator.com, ashoc.com, www.ashoc.com, a-shoc.myshopify.com) but the issuer and every endpoint are on shopify.com. The company operates no authorization server of its own.
  openIdConnectUrl: https://www.drinkaccelerator.com/.well-known/openid-configuration
  pkce:
  - S256
  provider: Shopify Customer Accounts (shop id 7133691957)
  response_types:
  - code
  subject_types:
  - public
  tokenUrl: https://shopify.com/authentication/7133691957/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
- flows:
  - authorizationUrl: https://shopify.com/authentication/7133691957/oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://shopify.com/authentication/7133691957/oauth/token
  name: shopify-customer-account-oauth2
  note: The RFC 8414 metadata document is byte-identical to the OIDC discovery document.
  source: https://www.drinkaccelerator.com/.well-known/oauth-authorization-server
  type: oauth2
- applies_to: https://www.drinkaccelerator.com/api/2026-07/graphql.json
  in: header
  name: customer-access-token
  note: Documented by the platform vendor, not by this company.
  observed: Required by the customer query field per the introspected schema; obtained via customerAccessTokenCreate.
  parameter: X-Shopify-Customer-Access-Token
  type: apiKey
slug: adrenalineshoc-authentication
source_filename: adrenalineshoc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource:\n- https://www.drinkaccelerator.com/.well-known/openid-configuration\n- https://www.drinkaccelerator.com/.well-known/oauth-authorization-server\n- https://www.drinkaccelerator.com/api/ucp/mcp\n- https://www.drinkaccelerator.com/api/2026-07/graphql.json\ndocs: https://www.drinkaccelerator.com/agents.md\nnote: >-\n  Derived from live probes, not from an OpenAPI document - this company publishes no\n  spec. derive-authentication.py found 0 schemes because there is no openapi/\n  directory; this file records the auth model actually observed on the wire.\nsummary:\n  types: [none, oauth2, openIdConnect, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\n  anonymous_surfaces: 3\nschemes:\n- name: anonymous-ucp-mcp\n  type: none\n  applies_to: https://www.drinkaccelerator.com/api/ucp/mcp\n  observed: tools/list returned HTTP 200 with all thirteen tools and their input schemas\n    without\
  \ any credential.\n  note: >-\n    tools/call is not anonymous in practice - it requires meta.ucp-agent.profile to\n    be a resolvable URI. That is an agent-identity control, not an authentication\n    control: no secret is exchanged and no account exists. Payment additionally\n    enforces a human buyer-approval invariant, which is a policy control.\n- name: anonymous-storefront-graphql\n  type: none\n  applies_to: https://www.drinkaccelerator.com/api/2026-07/graphql.json\n  observed: Full introspection returned HTTP 200 (428 types) with no X-Shopify-Storefront-Access-Token\n    header. Versions 2026-07, 2026-04, 2025-01 and 2024-04 all answer anonymously.\n  note: Customer-scoped fields still require a customerAccessToken obtained via the\n    customerAccessTokenCreate mutation.\n- name: anonymous-storefront-json\n  type: none\n  applies_to: https://www.drinkaccelerator.com/\n  observed: /products.json and /collections/all/products.json returned HTTP 200 unauthenticated\n    (both empty).\n\
  - name: shopify-customer-accounts-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://www.drinkaccelerator.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/7133691957\n  authorizationUrl: https://shopify.com/authentication/7133691957/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/7133691957/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/7133691957/logout\n  jwks_uri: https://shopify.com/authentication/7133691957/.well-known/jwks.json\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  pkce: [S256]\n  id_token_signing_alg: [RS256]\n  subject_types: [public]\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  applies_to: Customer account sign-in on the Accelerator Active Energy storefront\n  provider: Shopify Customer Accounts (shop id 7133691957)\n\
  \  note: >-\n    The discovery document is served from the company's own hosts (www.drinkaccelerator.com,\n    drinkaccelerator.com, ashoc.com, www.ashoc.com, a-shoc.myshopify.com) but the\n    issuer and every endpoint are on shopify.com. The company operates no\n    authorization server of its own.\n- name: shopify-customer-account-oauth2\n  type: oauth2\n  source: https://www.drinkaccelerator.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/7133691957/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/7133691957/oauth/token\n    scopes: 4\n  note: The RFC 8414 metadata document is byte-identical to the OIDC discovery document.\n- name: customer-access-token\n  type: apiKey\n  in: header\n  parameter: X-Shopify-Customer-Access-Token\n  applies_to: https://www.drinkaccelerator.com/api/2026-07/graphql.json\n  observed: Required by the customer query field per the introspected schema;\
  \ obtained\n    via customerAccessTokenCreate.\n  note: Documented by the platform vendor, not by this company.\nagent_identity:\n  mechanism: UCP agent profile\n  field: meta.ucp-agent.profile\n  format: URI\n  required_on: every tools/call\n  enforcement: HTTP 422 with JSON-RPC -32001 invalid_profile_url when absent - observed\n    live.\nx-evidence:\n- url: https://www.drinkaccelerator.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n- url: https://www.drinkaccelerator.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n- url: https://www.drinkaccelerator.com/api/ucp/mcp\n  http_status: 200\n  note: anonymous tools/list\n- url: https://www.drinkaccelerator.com/api/ucp/mcp\n  http_status: 422\n  note: tools/call without an agent profile\n- url: https://www.drinkaccelerator.com/api/2026-07/graphql.json\n  http_status: 200\n  note: anonymous full introspection\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adrenalineshoc/refs/heads/main/authentication/adrenalineshoc-authentication.yml
summary_line: none/oauth2/openIdConnect/apiKey · 6 schemes
tags:
- Company
- Beverage
- Energy Drinks
- Consumer Packaged Goods
- Retail
- E-Commerce
- Direct to Consumer
- Agentic Commerce
- Shopify
- Sports Nutrition
---
