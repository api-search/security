---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Chill Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Chill secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Chill
provider_slug: chill
scheme_count: 2
schemes:
- authorization_endpoint: https://shopify.com/authentication/56172019867/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://shopify.com/authentication/56172019867/logout
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  jwks_uri: https://shopify.com/authentication/56172019867/.well-known/jwks.json
  name: ShopifyCustomerAccountOAuth
  sources:
  - well-known/chill-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/56172019867/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: oauth2
- claims:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://chill.com/.well-known/openid-configuration
  sources:
  - well-known/chill-openid-configuration.json
  subject_types:
  - public
  type: openIdConnect
slug: chill-authentication
source_filename: chill-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://chill.com/.well-known/openid-configuration\ndocs: https://chill.com/.well-known/openid-configuration\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  provider: Shopify Customer Account\n  issuer: https://shopify.com/authentication/56172019867\n  notes: >-\n    Chill.com runs on Shopify; end-user / customer authentication is Shopify\n    Customer Account OAuth 2.0 + OpenID Connect. Agent commerce over the UCP MCP\n    endpoint reuses these customer-account scopes. Read-only catalog browsing\n    requires no authentication.\nschemes:\n- name: ShopifyCustomerAccountOAuth\n  type: oauth2\n  flow: authorizationCode\n  authorization_endpoint: https://shopify.com/authentication/56172019867/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/56172019867/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/56172019867/logout\n  jwks_uri: https://shopify.com/authentication/56172019867/.well-known/jwks.json\n\
  \  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [client_secret_basic]\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  id_token_signing_alg: [RS256]\n  sources: [well-known/chill-openid-configuration.json]\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://chill.com/.well-known/openid-configuration\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  subject_types: [public]\n  sources: [well-known/chill-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chill/refs/heads/main/authentication/chill-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Wellness
- Supplements
- E-commerce
- Marketplace
- Health
- Agentic Commerce
- Shopify
- Retail
- MCP
---
