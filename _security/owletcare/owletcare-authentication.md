---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Owletcare Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Owletcare secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Owletcare
provider_slug: owletcare
scheme_count: 1
schemes:
- authorization_endpoint: https://b2b.owletcare.com/authentication/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://b2b.owletcare.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/10043036
  jwks_uri: https://b2b.owletcare.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://owletcare.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/owletcare-openid-configuration.json
  token_endpoint: https://b2b.owletcare.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: owletcare-authentication
source_filename: owletcare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://owletcare.com/.well-known/openid-configuration\nnotes: >-\n  Derived from the live OIDC discovery document served at owletcare.com. The\n  authentication surface is Shopify's Customer Account API (issuer\n  https://shopify.com/authentication/10043036); Owlet does not publish a\n  first-party developer API of its own.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/10043036\n  openIdConnectUrl: https://owletcare.com/.well-known/openid-configuration\n  authorization_endpoint: https://b2b.owletcare.com/authentication/oauth/authorize\n  token_endpoint: https://b2b.owletcare.com/authentication/oauth/token\n  end_session_endpoint: https://b2b.owletcare.com/authentication/logout\n  jwks_uri: https://b2b.owletcare.com/authentication/.well-known/jwks.json\n\
  \  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  id_token_signing_alg_values_supported:\n  - RS256\n  code_challenge_methods_supported:\n  - S256\n  sources:\n  - well-known/owletcare-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/owletcare/refs/heads/main/authentication/owletcare-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Baby Care
- Health Monitoring
- Consumer Electronics
- Connected Devices
- IoT
- Sleep
- Wearables
---
