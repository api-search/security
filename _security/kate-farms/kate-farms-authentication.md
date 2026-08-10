---
api_key_in:
- header
auth_types:
- openIdConnect
- oauth2
- apiKey
- none
description: ''
kind: authentication
layout: security
method: probed
name: Kate Farms Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Kate Farms secures its APIs with openIdConnect, oauth2, apiKey, and none across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Kate Farms
provider_slug: kate-farms
scheme_count: 5
schemes:
- description: The Storefront GraphQL endpoint at https://shop.katefarms.com/api/2026-01/graphql.json answered queries AND a full introspection query with no credential of any kind on 2026-08-04. Public catalog, collection, search, blog, page and metaobject reads require no authentication.
  name: AnonymousStorefront
  sources:
  - graphql/kate-farms-storefront.graphql
  type: none
  verified: '2026-08-04'
- description: Shopify's documented public storefront credential for the Storefront API. Not required for the anonymous reads observed here, but it is the documented scheme for the surface and is the credential a first-party client uses.
  in: header
  name: StorefrontAccessToken
  parameter_name: X-Shopify-Storefront-Access-Token
  sources:
  - https://shopify.dev/docs/api/storefront
  type: apiKey
  x-note: Documented by the platform (Shopify), not by Kate Farms.
- authorization_endpoint: https://shopify.com/authentication/2056802/oauth/authorize
  claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  code_challenge_methods_supported:
  - S256
  description: Kate Farms' shopper identity. Customer Accounts sign-in is an OIDC authorization-code flow with mandatory PKCE (S256) against a per-shop Shopify issuer. Scopes are catalogued in scopes/kate-farms-scopes.yml.
  end_session_endpoint: https://shopify.com/authentication/2056802/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/2056802
  jwks_uri: https://shopify.com/authentication/2056802/.well-known/jwks.json
  name: CustomerAccountsOIDC
  openIdConnectUrl: https://shop.katefarms.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/kate-farms-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://shopify.com/authentication/2056802/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
  verified: '2026-08-04'
- description: The Storefront schema also carries a legacy customer access token model — customerAccessTokenCreate / Renew / Delete mutations mint a CustomerAccessToken passed as a GraphQL argument to customer-scoped queries and mutations. Present in the live schema alongside the newer OIDC Customer Accounts flow.
  in: header
  name: CustomerAccessToken
  parameter_name: customerAccessToken (GraphQL argument)
  sources:
  - graphql/kate-farms-storefront.graphql
  type: apiKey
  verified: '2026-08-04'
- authorization_server: https://shopify.com/authentication/2056802
  bearer_methods_supported:
  - header
  description: The UCP MCP endpoint at https://shop.katefarms.com/api/ucp/mcp requires a resolvable agent profile URI before it will answer tools/list. Anonymous calls (with and without MCP-Protocol-Version / UCP-Version headers) returned JSON-RPC error -32001 "UCP discovery failed" with data.code invalid_profile_url. Bearer tokens for the protected resource https://shop.katefarms.com are issued by the authorization server declared at /.well-known/oauth-protected-resource, presented in the Authorization header.
  gated: true
  name: UCPAgentProfile
  sources:
  - well-known/kate-farms-oauth-protected-resource.json
  - well-known/kate-farms-ucp.json
  type: oauth2
  verified: '2026-08-04'
slug: kate-farms-authentication
source_filename: kate-farms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://shop.katefarms.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  - apiKey\n  - none\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  bearer_methods_supported:\n  - header\nschemes:\n- name: AnonymousStorefront\n  type: none\n  description: The Storefront GraphQL endpoint at https://shop.katefarms.com/api/2026-01/graphql.json\n    answered queries AND a full introspection query with no credential of any kind\n    on 2026-08-04. Public catalog, collection, search, blog, page and metaobject reads\n    require no authentication.\n  sources:\n  - graphql/kate-farms-storefront.graphql\n  verified: '2026-08-04'\n- name: StorefrontAccessToken\n  type: apiKey\n  in: header\n  parameter_name: X-Shopify-Storefront-Access-Token\n  description: Shopify's documented public storefront credential for the Storefront\n    API. Not\
  \ required for the anonymous reads observed here, but it is the documented\n    scheme for the surface and is the credential a first-party client uses.\n  sources:\n  - https://shopify.dev/docs/api/storefront\n  x-note: Documented by the platform (Shopify), not by Kate Farms.\n- name: CustomerAccountsOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://shop.katefarms.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/2056802\n  authorization_endpoint: https://shopify.com/authentication/2056802/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/2056802/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/2056802/logout\n  jwks_uri: https://shopify.com/authentication/2056802/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n\
  \  code_challenge_methods_supported:\n  - S256\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  claims_supported:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n  description: Kate Farms' shopper identity. Customer Accounts sign-in is an OIDC\n    authorization-code flow with mandatory PKCE (S256) against a per-shop Shopify issuer.\n    Scopes are catalogued in scopes/kate-farms-scopes.yml.\n  sources:\n  - well-known/kate-farms-openid-configuration.json\n  verified: '2026-08-04'\n- name: CustomerAccessToken\n  type: apiKey\n  in: header\n  parameter_name: 'customerAccessToken (GraphQL argument)'\n  description: The Storefront schema also carries a legacy customer access token model\n    — customerAccessTokenCreate / Renew / Delete mutations mint a CustomerAccessToken\n    passed as a GraphQL argument to customer-scoped queries and mutations. Present\n    in the live schema alongside the newer\
  \ OIDC Customer Accounts flow.\n  sources:\n  - graphql/kate-farms-storefront.graphql\n  verified: '2026-08-04'\n- name: UCPAgentProfile\n  type: oauth2\n  description: The UCP MCP endpoint at https://shop.katefarms.com/api/ucp/mcp requires\n    a resolvable agent profile URI before it will answer tools/list. Anonymous calls\n    (with and without MCP-Protocol-Version / UCP-Version headers) returned JSON-RPC\n    error -32001 \"UCP discovery failed\" with data.code invalid_profile_url. Bearer\n    tokens for the protected resource https://shop.katefarms.com are issued by the\n    authorization server declared at /.well-known/oauth-protected-resource, presented\n    in the Authorization header.\n  authorization_server: https://shopify.com/authentication/2056802\n  bearer_methods_supported:\n  - header\n  gated: true\n  sources:\n  - well-known/kate-farms-oauth-protected-resource.json\n  - well-known/kate-farms-ucp.json\n  verified: '2026-08-04'\nx-evidence:\n- url: https://shop.katefarms.com/.well-known/openid-configuration\n\
  \  http_status: 200\n- url: https://shop.katefarms.com/.well-known/oauth-protected-resource\n  http_status: 200\n- url: https://shop.katefarms.com/api/2026-01/graphql.json\n  http_status: 200\n  note: anonymous introspection succeeded, 424 types returned\n- url: https://shop.katefarms.com/api/ucp/mcp\n  http_status: 422\n  note: 'JSON-RPC -32001 invalid_profile_url: \"Unable to fetch agent profile: Missing\n    profile uri\"'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kate-farms/refs/heads/main/authentication/kate-farms-authentication.yml
summary_line: openIdConnect/oauth2/apiKey/none · 5 schemes
tags:
- Company
- Nutrition
- Medical Nutrition
- Health
- Food and Beverage
- Consumer Packaged Goods
- E-Commerce
- Agentic Commerce
- Retail
- Shopify
- GraphQL
---
