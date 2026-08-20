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
name: 100 Thieves Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: 100 Thieves secures its APIs with none, oauth2, and openIdConnect across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: 100 Thieves
provider_slug: 100-thieves
scheme_count: 6
schemes:
- applies_to: https://100thieves.com/api/ucp/mcp
  name: anonymous-ucp-mcp
  note: Transacting tools still enforce a buyer-approval invariant at payment; that is a policy control, not an authentication control.
  observed: tools/list returned HTTP 200 with the full tool set and input schemas without any credential.
  type: none
- applies_to: https://100thieves.com/api/2024-04/graphql.json
  name: anonymous-storefront-graphql
  note: Customer-scoped fields still require a customerAccessToken obtained via the customerAccessTokenCreate mutation.
  observed: Full introspection returned HTTP 200 (414 types) with no X-Shopify-Storefront-Access-Token header.
  type: none
- applies_to: https://100thieves.com/
  name: anonymous-storefront-json
  observed: /collections/all/products.json returned HTTP 200 unauthenticated.
  type: none
- applies_to: Customer account sign-in at https://100thieves.com/account/login
  authorizationUrl: https://shopify.com/authentication/31052262/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/31052262/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/31052262
  jwks_uri: https://shopify.com/authentication/31052262/.well-known/jwks.json
  name: shopify-customer-accounts-oidc
  openIdConnectUrl: https://100thieves.com/.well-known/openid-configuration
  pkce:
  - S256
  provider: Shopify Customer Accounts (shop id 31052262)
  response_types:
  - code
  subject_types:
  - public
  tokenUrl: https://shopify.com/authentication/31052262/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- flows:
  - authorizationUrl: https://shopify.com/authentication/31052262/oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://shopify.com/authentication/31052262/oauth/token
  name: shopify-customer-account-oauth2
  note: The RFC 8414 metadata document is byte-identical to the OIDC discovery document.
  source: https://100thieves.com/.well-known/oauth-authorization-server
  type: oauth2
- applies_to: https://100thieves.com/api/2024-04/graphql.json
  in: header
  name: customer-access-token
  note: Documented by the platform vendor, not by 100 Thieves.
  observed: Required by the customer query field per the introspected schema; obtained via customerAccessTokenCreate.
  parameter: X-Shopify-Customer-Access-Token
  type: apiKey
slug: 100-thieves-authentication
source_filename: 100-thieves-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource:\n- https://100thieves.com/.well-known/openid-configuration\n- https://100thieves.com/.well-known/oauth-authorization-server\n- https://100thieves.com/api/ucp/mcp\n- https://100thieves.com/api/2024-04/graphql.json\ndocs: https://100thieves.com/agents.md\nnote: >-\n  Derived from live probes, not from an OpenAPI document — 100 Thieves publishes no\n  spec. derive-authentication.py found 0 schemes because there is no openapi/ directory;\n  this file records the auth model actually observed on the wire.\nsummary:\n  types: [none, oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\n  anonymous_surfaces: 3\nschemes:\n- name: anonymous-ucp-mcp\n  type: none\n  applies_to: https://100thieves.com/api/ucp/mcp\n  observed: tools/list returned HTTP 200 with the full tool set and input schemas without\n    any credential.\n  note: Transacting tools still enforce a buyer-approval invariant\
  \ at payment; that\n    is a policy control, not an authentication control.\n- name: anonymous-storefront-graphql\n  type: none\n  applies_to: https://100thieves.com/api/2024-04/graphql.json\n  observed: Full introspection returned HTTP 200 (414 types) with no X-Shopify-Storefront-Access-Token\n    header.\n  note: Customer-scoped fields still require a customerAccessToken obtained via the\n    customerAccessTokenCreate mutation.\n- name: anonymous-storefront-json\n  type: none\n  applies_to: https://100thieves.com/\n  observed: /collections/all/products.json returned HTTP 200 unauthenticated.\n- name: shopify-customer-accounts-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://100thieves.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/31052262\n  authorizationUrl: https://shopify.com/authentication/31052262/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/31052262/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/31052262/logout\n\
  \  jwks_uri: https://shopify.com/authentication/31052262/.well-known/jwks.json\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  token_endpoint_auth_methods: [client_secret_basic]\n  pkce: [S256]\n  id_token_signing_alg: [RS256]\n  subject_types: [public]\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  applies_to: Customer account sign-in at https://100thieves.com/account/login\n  provider: Shopify Customer Accounts (shop id 31052262)\n- name: shopify-customer-account-oauth2\n  type: oauth2\n  source: https://100thieves.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/31052262/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/31052262/oauth/token\n    scopes: 4\n  note: The RFC 8414 metadata document is byte-identical to the OIDC discovery document.\n- name: customer-access-token\n\
  \  type: apiKey\n  in: header\n  parameter: X-Shopify-Customer-Access-Token\n  applies_to: https://100thieves.com/api/2024-04/graphql.json\n  observed: Required by the customer query field per the introspected schema; obtained\n    via customerAccessTokenCreate.\n  note: Documented by the platform vendor, not by 100 Thieves.\nx-evidence:\n- url: https://100thieves.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n- url: https://100thieves.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n- url: https://100thieves.com/api/ucp/mcp\n  http_status: 200\n  note: anonymous tools/list\n- url: https://100thieves.com/api/2024-04/graphql.json\n  http_status: 200\n  note: anonymous full introspection\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/100-thieves/refs/heads/main/authentication/100-thieves-authentication.yml
summary_line: none/oauth2/openIdConnect · 6 schemes
tags:
- Company
- Esports
- Gaming
- Apparel
- Retail
- E-Commerce
- Entertainment
- Media
- Direct to Consumer
- Agentic Commerce
---
