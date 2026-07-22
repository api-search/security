---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Nimasensor Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: NimaSensor secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: NimaSensor
provider_slug: nimasensor
scheme_count: 1
schemes:
- authorizationUrl: https://account.nimanow.com/authentication/oauth/authorize
  end_session_endpoint: https://account.nimanow.com/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/61165174846
  jwks_uri: https://account.nimanow.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://nimanow.com/.well-known/openid-configuration
  pkce:
  - S256
  response_types:
  - code
  sources:
  - well-known/nimasensor-openid-configuration.json
  tokenUrl: https://account.nimanow.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: nimasensor-authentication
source_filename: nimasensor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://nimanow.com/.well-known/openid-configuration\nnote: >-\n  Auth surface is Shopify's Customer Account API (platform-level), discovered from the store's\n  OIDC configuration - not a first-party NIMA developer API. Enables end-customer login to the\n  NIMA storefront. Included because it is a genuine, publicly discoverable authentication surface\n  on the provider domain.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  issuer: https://shopify.com/authentication/61165174846\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://nimanow.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/61165174846\n  authorizationUrl: https://account.nimanow.com/authentication/oauth/authorize\n  tokenUrl: https://account.nimanow.com/authentication/oauth/token\n  end_session_endpoint: https://account.nimanow.com/authentication/logout\n\
  \  jwks_uri: https://account.nimanow.com/authentication/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  pkce:\n  - S256\n  id_token_signing_alg:\n  - RS256\n  sources:\n  - well-known/nimasensor-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nimasensor/refs/heads/main/authentication/nimasensor-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Health
- Consumer Hardware
- Food Safety
- Gluten
- Celiac
- E-Commerce
- IoT
---
