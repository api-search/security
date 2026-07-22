---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Beeline Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Beeline secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Beeline
provider_slug: beeline
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/18978919/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://shopify.com/authentication/18978919/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/18978919
  jwks_uri: https://shopify.com/authentication/18978919/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://beeline.co/.well-known/openid-configuration
  response_types:
  - code
  token_endpoint: https://shopify.com/authentication/18978919/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: beeline-authentication
source_filename: beeline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://beeline.co/.well-known/openid-configuration\nnote: >-\n  Authentication surface on the Beeline storefront is provided by Shopify\n  customer accounts (OpenID Connect / OAuth 2.0). There is no separate\n  first-party Beeline developer-API auth scheme published. The UCP shopping MCP\n  endpoint operates under buyer-approved checkout rather than developer API keys.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  pkce: true\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/18978919\n  openIdConnectUrl: https://beeline.co/.well-known/openid-configuration\n  authorization_endpoint: https://shopify.com/authentication/18978919/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/18978919/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/18978919/logout\n  jwks_uri: https://shopify.com/authentication/18978919/.well-known/jwks.json\n\
  \  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  code_challenge_methods:\n  - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  id_token_signing_alg:\n  - RS256\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beeline/refs/heads/main/authentication/beeline-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Navigation
- Cycling
- Motorcycle
- Hardware
- GPS
- Location
- Maps
- Mobile App
- Consumer Electronics
- Ecommerce
---
