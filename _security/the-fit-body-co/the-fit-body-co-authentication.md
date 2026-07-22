---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: The Fit Body Co (fitbody.mx) is a Shopify-hosted storefront and publishes no first-party developer API. The only authentication surface exposed on the host is Shopify's Customer Account API, whose OpenID Connect discovery document is served at /.well-known/openid-configuration (and /.well-known/oauth-authorization-server) with issuer https://shopify.com/authentication/24443367. This profile captures that OIDC/OAuth 2.0 surface verbatim from the live discovery document; it is a Shopify platform capability scoped to this shop, not a bespoke Fit Body Co API.
kind: authentication
layout: security
method: searched
name: The Fit Body Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Fit Body Co secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Fit Body Co
provider_slug: the-fit-body-co
scheme_count: 1
schemes:
- authorizationUrl: https://shopify.com/authentication/24443367/oauth/authorize
  code_challenge_methods:
  - S256
  endSessionEndpoint: https://shopify.com/authentication/24443367/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/24443367
  jwksUri: https://shopify.com/authentication/24443367/.well-known/jwks.json
  name: shopifyCustomerAccountOIDC
  openIdConnectUrl: https://fitbody.mx/.well-known/openid-configuration
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  source: https://fitbody.mx/.well-known/openid-configuration
  tokenUrl: https://shopify.com/authentication/24443367/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: the-fit-body-co-authentication
source_filename: the-fit-body-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://fitbody.mx/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\ndescription: >-\n  The Fit Body Co (fitbody.mx) is a Shopify-hosted storefront and publishes no\n  first-party developer API. The only authentication surface exposed on the host\n  is Shopify's Customer Account API, whose OpenID Connect discovery document is\n  served at /.well-known/openid-configuration (and /.well-known/oauth-authorization-server)\n  with issuer https://shopify.com/authentication/24443367. This profile captures\n  that OIDC/OAuth 2.0 surface verbatim from the live discovery document; it is a\n  Shopify platform capability scoped to this shop, not a bespoke Fit Body Co API.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\nschemes:\n- name: shopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://fitbody.mx/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/24443367\n\
  \  authorizationUrl: https://shopify.com/authentication/24443367/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/24443367/oauth/token\n  jwksUri: https://shopify.com/authentication/24443367/.well-known/jwks.json\n  endSessionEndpoint: https://shopify.com/authentication/24443367/logout\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  code_challenge_methods:\n  - S256\n  id_token_signing_alg:\n  - RS256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  source: https://fitbody.mx/.well-known/openid-configuration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-fit-body-co/refs/heads/main/authentication/the-fit-body-co-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Sports Nutrition
- Dietary Supplements
- E-commerce
- Health and Wellness
- Consumer Products
- Mexico
- Shopify
---
