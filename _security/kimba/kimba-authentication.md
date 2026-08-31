---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Kimba Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Kimba secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Kimba
provider_slug: kimba
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/76759498890/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/76759498890/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  issuer: https://shopify.com/authentication/76759498890
  name: ShopifyCustomerAccountOIDC
  response_types_supported:
  - code
  sources:
  - well-known/kimba-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/76759498890/oauth/token
  token_endpoint_auth_methods_supported_note: see published openid-configuration
  type: openIdConnect
slug: kimba-authentication
source_filename: kimba-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://kimba.ai/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  Kimba runs on Shopify; buyer/customer authentication is handled by the Shopify\n  Customer Account API, an OpenID Connect provider. Values below are transcribed\n  verbatim from the store's published OIDC discovery document. Read-only storefront\n  browsing (products/collections/search JSON) requires no authentication.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\n  pkce: true\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/76759498890\n  authorization_endpoint: https://shopify.com/authentication/76759498890/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/76759498890/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/76759498890/logout\n  grant_types_supported:\
  \ [authorization_code, refresh_token, \"urn:ietf:params:oauth:grant-type:jwt-bearer\"]\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported_note: see published openid-configuration\n  sources: [well-known/kimba-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kimba/refs/heads/main/authentication/kimba-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Sleep Technology
- Consumer Hardware
- Health & Wellness
- Artificial Intelligence
- Wearables
- E-Commerce
- Agentic Commerce
---
