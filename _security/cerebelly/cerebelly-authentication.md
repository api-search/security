---
api_key_in: []
auth_types: []
description: 'Cerebelly publishes no OpenAPI, so this profile is built from the OpenID Connect and OAuth metadata documents its own host serves, plus the observed behaviour of each live endpoint. Three distinct authentication postures coexist on the domain: the commerce agent surfaces are anonymous, the customer-account surface is a full OIDC authorization-code flow with PKCE, and payment authorization is delegated entirely to buyer-approved payment handlers.'
kind: authentication
layout: security
method: searched
name: Cerebelly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cerebelly declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Cerebelly
provider_slug: cerebelly
scheme_count: 4
schemes:
- applies_to:
  - https://cerebelly.com/api/ucp/mcp
  - https://cerebelly.com/api/2026-01/graphql.json
  - https://cerebelly.com/products.json
  - https://cerebelly.com/collections/{handle}/products.json
  description: Catalog discovery, MCP tools/list, GraphQL introspection and the JSON product endpoints all answer HTTP 200 with no credential of any kind. Verified anonymously on 2026-08-09.
  evidence:
    authenticated: false
    http_status: 200
    url: https://cerebelly.com/api/ucp/mcp
  id: none-anonymous
  type: none
- applies_to:
  - https://account.cerebelly.com/customer/api/2026-01/graphql
  authorization_endpoint: https://account.cerebelly.com/authentication/oauth/authorize
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
  code_challenge_methods:
  - S256
  description: Shopify customer accounts. Authorization code flow with PKCE; the customer account GraphQL API returns HTTP 401 without a bearer token.
  end_session_endpoint: https://account.cerebelly.com/authentication/logout
  evidence:
    authenticated: false
    http_status: 401
    url: https://account.cerebelly.com/customer/api/2026-01/graphql
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-storefront-oidc
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/74590912725
  jwks_uri: https://account.cerebelly.com/authentication/.well-known/jwks.json
  openIdConnectUrl: https://cerebelly.com/.well-known/openid-configuration
  response_types:
  - code
  scopes: ../scopes/cerebelly-scopes.yml
  subject_types:
  - public
  token_endpoint: https://account.cerebelly.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- applies_to:
  - https://cerebelly.com/api/2026-01/graphql.json
  derived_from: graphql/cerebelly-storefront.graphql
  description: Optional per-request customer token on the Storefront API, minted by the customerAccessTokenCreate mutation. Required only for the customer query and the customer* mutations; every catalog and cart field works without it.
  header: Shopify-Storefront-Customer-Access-Token
  id: storefront-customer-access-token
  scheme: bearer
  type: http
- applies_to:
  - https://cerebelly.com/api/ucp/mcp (complete_checkout)
  description: Payment is not authenticated by the API caller. complete_checkout accepts a payment instrument minted by one of three configured UCP payment handlers, and both llms.txt and robots.txt state that an agent must not finalize payment without an explicit, contemporaneous human approval step.
  handlers:
  - com.google.pay (gpay)
  - dev.shopify.card (shopify.card)
  - dev.shopify.shop_pay (shop_pay)
  id: ucp-payment-handler
  source: https://cerebelly.com/.well-known/ucp
  type: delegated
slug: cerebelly-authentication
source_filename: cerebelly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://cerebelly.com/.well-known/openid-configuration\ndocs: https://cerebelly.com/agents.md\nname: Cerebelly authentication profile\ndescription: >-\n  Cerebelly publishes no OpenAPI, so this profile is built from the OpenID Connect\n  and OAuth metadata documents its own host serves, plus the observed behaviour of\n  each live endpoint. Three distinct authentication postures coexist on the domain:\n  the commerce agent surfaces are anonymous, the customer-account surface is a full\n  OIDC authorization-code flow with PKCE, and payment authorization is delegated\n  entirely to buyer-approved payment handlers.\nschemes:\n- id: none-anonymous\n  type: none\n  applies_to:\n  - https://cerebelly.com/api/ucp/mcp\n  - https://cerebelly.com/api/2026-01/graphql.json\n  - https://cerebelly.com/products.json\n  - https://cerebelly.com/collections/{handle}/products.json\n  description: >-\n    Catalog discovery, MCP tools/list, GraphQL\
  \ introspection and the JSON product\n    endpoints all answer HTTP 200 with no credential of any kind. Verified\n    anonymously on 2026-08-09.\n  evidence:\n    url: https://cerebelly.com/api/ucp/mcp\n    http_status: 200\n    authenticated: false\n- id: shopify-storefront-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://cerebelly.com/.well-known/openid-configuration\n  applies_to:\n  - https://account.cerebelly.com/customer/api/2026-01/graphql\n  description: >-\n    Shopify customer accounts. Authorization code flow with PKCE; the customer\n    account GraphQL API returns HTTP 401 without a bearer token.\n  issuer: https://shopify.com/authentication/74590912725\n  authorization_endpoint: https://account.cerebelly.com/authentication/oauth/authorize\n  token_endpoint: https://account.cerebelly.com/authentication/oauth/token\n  end_session_endpoint: https://account.cerebelly.com/authentication/logout\n  jwks_uri: https://account.cerebelly.com/authentication/.well-known/jwks.json\n\
  \  grant_types:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  response_types:\n  - code\n  code_challenge_methods:\n  - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  id_token_signing_alg:\n  - RS256\n  subject_types:\n  - public\n  claims:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n  scopes: ../scopes/cerebelly-scopes.yml\n  evidence:\n    url: https://account.cerebelly.com/customer/api/2026-01/graphql\n    http_status: 401\n    authenticated: false\n- id: storefront-customer-access-token\n  type: http\n  scheme: bearer\n  header: Shopify-Storefront-Customer-Access-Token\n  applies_to:\n  - https://cerebelly.com/api/2026-01/graphql.json\n  description: >-\n    Optional per-request customer token on the Storefront API, minted by the\n    customerAccessTokenCreate mutation. Required only for the customer query and\n    the customer* mutations; every catalog and cart\
  \ field works without it.\n  derived_from: graphql/cerebelly-storefront.graphql\n- id: ucp-payment-handler\n  type: delegated\n  applies_to:\n  - https://cerebelly.com/api/ucp/mcp (complete_checkout)\n  description: >-\n    Payment is not authenticated by the API caller. complete_checkout accepts a\n    payment instrument minted by one of three configured UCP payment handlers, and\n    both llms.txt and robots.txt state that an agent must not finalize payment\n    without an explicit, contemporaneous human approval step.\n  handlers:\n  - com.google.pay (gpay)\n  - dev.shopify.card (shopify.card)\n  - dev.shopify.shop_pay (shop_pay)\n  source: https://cerebelly.com/.well-known/ucp\nprotected_resource_metadata:\n  url: https://cerebelly.com/.well-known/oauth-protected-resource\n  rfc: RFC 9728\n  resource: https://cerebelly.com\n  authorization_servers:\n  - https://account.cerebelly.com\n  - https://shopify.com/authentication/74590912725\n  bearer_methods_supported:\n  - header\nnotes:\n\
  - >-\n  There is no API key, no developer registration, and no partner program. Cerebelly\n  does not run a developer platform — the authenticated surface it exposes is the\n  Shopify customer-account layer for its own shoppers.\n- >-\n  The MCP endpoint answers tools/list anonymously, which is the exception rather\n  than the rule across the catalog; most MCP surfaces return an OAuth challenge.\nx-evidence:\n  fetched: '2026-08-09'\n  urls:\n  - url: https://cerebelly.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://cerebelly.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://cerebelly.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://account.cerebelly.com/customer/api/2026-01/graphql\n    http_status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerebelly/refs/heads/main/authentication/cerebelly-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Baby Food
- Consumer Packaged Goods
- Food and Beverage
- E-Commerce
- Retail
- Direct to Consumer
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- Nutrition
---
