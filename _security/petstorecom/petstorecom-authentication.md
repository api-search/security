---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Petstorecom Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Petstore.com secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Petstore.com
provider_slug: petstorecom
scheme_count: 1
schemes:
- authorizationUrl: https://shopify.com/authentication/27249049675/oauth/authorize
  code_challenge_methods:
  - S256
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/27249049675
  jwks_uri: https://shopify.com/authentication/27249049675/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://petstore.com/.well-known/openid-configuration
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/petstorecom-openid-configuration.json
  tokenUrl: https://shopify.com/authentication/27249049675/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: petstorecom-authentication
source_filename: petstorecom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://petstore.com/.well-known/openid-configuration\ndocs: https://petstore.com/agents.md\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  notes: >-\n    Buyer identity and the agent-facing MCP surface authenticate via Shopify\n    Customer Account OpenID Connect. Read-only storefront browsing (products,\n    collections, search, sitemap) requires no authentication. Payment always\n    requires contemporaneous human approval regardless of auth.\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://petstore.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/27249049675\n    authorizationUrl: https://shopify.com/authentication/27249049675/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/27249049675/oauth/token\n    jwks_uri: https://shopify.com/authentication/27249049675/.well-known/jwks.json\n\
  \    grant_types: [authorization_code, refresh_token, \"urn:ietf:params:oauth:grant-type:jwt-bearer\"]\n    response_types: [code]\n    code_challenge_methods: [S256]\n    token_endpoint_auth_methods: [client_secret_basic]\n    id_token_signing_alg: [RS256]\n    scopes:\n      - openid\n      - email\n      - customer-account-api:full\n      - customer-account-mcp-api:full\n    sources: [well-known/petstorecom-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/petstorecom/refs/heads/main/authentication/petstorecom-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Commerce
- E-commerce
- Retail
- Pet Supplies
- Agentic Commerce
- UCP
- MCP
- Shopify
---
