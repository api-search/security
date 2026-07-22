---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tenlittle Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Ten Little secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Ten Little
provider_slug: tenlittle
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/26030735465/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/26030735465/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/26030735465
  jwks_uri: https://shopify.com/authentication/26030735465/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://tenlittle.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/tenlittle-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/26030735465/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: tenlittle-authentication
source_filename: tenlittle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://tenlittle.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\n# Ten Little publishes no first-party developer API. The only authorization\n# surface reachable on the tenlittle.com domain is Shopify's platform-level\n# Customer Account OIDC/OAuth server (the store's shopper login), discovered\n# via /.well-known/openid-configuration. Captured verbatim from that document.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\n  first_party: false\n  provider: Shopify (Customer Account API)\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://tenlittle.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/26030735465\n  authorization_endpoint: https://shopify.com/authentication/26030735465/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/26030735465/oauth/token\n\
  \  end_session_endpoint: https://shopify.com/authentication/26030735465/logout\n  jwks_uri: https://shopify.com/authentication/26030735465/.well-known/jwks.json\n  id_token_signing_alg_values_supported: [RS256]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  code_challenge_methods_supported: [S256]\n  grant_types_supported: [authorization_code, refresh_token, \"urn:ietf:params:oauth:grant-type:jwt-bearer\"]\n  response_types_supported: [code]\n  sources: [well-known/tenlittle-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenlittle/refs/heads/main/authentication/tenlittle-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Retail
- E-commerce
- Consumer Goods
- Children
- Footwear
- Direct-to-Consumer
- Shopify
---
