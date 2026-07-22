---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Teabox Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Teabox secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Teabox
provider_slug: teabox
scheme_count: 1
schemes:
- authorization_endpoint: https://accounts.teabox.com/authentication/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://accounts.teabox.com/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/20013521
  jwks_uri: https://accounts.teabox.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://www.teabox.com/.well-known/openid-configuration
  response_types:
  - code
  sources:
  - well-known/teabox-openid-configuration.json
  token_endpoint: https://accounts.teabox.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: teabox-authentication
source_filename: teabox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.teabox.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  Teabox authenticates buyers through the Shopify Customer Account API, an\n  OpenID Connect provider. The OIDC issuer is brand-scoped to\n  accounts.teabox.com. Authorization Code flow with PKCE (S256) is used;\n  clients authenticate to the token endpoint with client_secret_basic. This is\n  a platform-provided identity surface rather than a first-party Teabox API.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.teabox.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/20013521\n  authorization_endpoint: https://accounts.teabox.com/authentication/oauth/authorize\n  token_endpoint: https://accounts.teabox.com/authentication/oauth/token\n\
  \  end_session_endpoint: https://accounts.teabox.com/authentication/logout\n  jwks_uri: https://accounts.teabox.com/authentication/.well-known/jwks.json\n  token_endpoint_auth_methods: [client_secret_basic]\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  id_token_signing_alg: [RS256]\n  code_challenge_methods: [S256]\n  sources: [well-known/teabox-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teabox/refs/heads/main/authentication/teabox-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Consumer
- Tea
- Food and Beverage
- E-commerce
- Retail
- Shopify
- Agent Commerce
---
