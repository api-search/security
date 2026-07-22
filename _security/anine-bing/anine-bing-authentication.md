---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Anine Bing Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Anine Bing secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Anine Bing
provider_slug: anine-bing
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/1501528/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/1501528/logout
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/1501528
  jwks_uri: https://shopify.com/authentication/1501528/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://aninebing.com/.well-known/openid-configuration
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/anine-bing-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/1501528/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: anine-bing-authentication
source_filename: anine-bing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://aninebing.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  notes: >-\n    Customer authentication for the Anine Bing storefront is handled by Shopify's\n    Customer Account API via OpenID Connect. The OIDC issuer is\n    https://shopify.com/authentication/1501528 (per the store's\n    /.well-known/openid-configuration). PKCE (S256) is required; token endpoint\n    auth is client_secret_basic; id_tokens are RS256-signed.\nschemes:\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://aninebing.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/1501528\n  authorization_endpoint: https://shopify.com/authentication/1501528/oauth/authorize\n\
  \  token_endpoint: https://shopify.com/authentication/1501528/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/1501528/logout\n  jwks_uri: https://shopify.com/authentication/1501528/.well-known/jwks.json\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  scopes_supported: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  sources: ['well-known/anine-bing-openid-configuration.json']\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anine-bing/refs/heads/main/authentication/anine-bing-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Retail
- Fashion
- Apparel
- Ecommerce
- Shopify
- Agent Commerce
- MCP
---
