---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Holy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: HOLY secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: HOLY
provider_slug: holy
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/47328854173/oauth/authorize
    codeChallengeMethods:
    - S256
    endSessionUrl: https://shopify.com/authentication/47328854173/logout
    flow: authorizationCode
    grantTypes:
    - authorization_code
    - refresh_token
    - urn:ietf:params:oauth:grant-type:jwt-bearer
    tokenEndpointAuthMethods:
    - client_secret_basic
    tokenUrl: https://shopify.com/authentication/47328854173/oauth/token
  issuer: https://shopify.com/authentication/47328854173
  name: shopify-customer-account-oauth2
  sources:
  - well-known/holy-openid-configuration.json
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
  idTokenSigningAlg:
  - RS256
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://de.holy.com/.well-known/openid-configuration
  sources:
  - well-known/holy-openid-configuration.json
  type: openIdConnect
slug: holy-authentication
source_filename: holy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://de.holy.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  notes: >-\n    Authentication is delegated to Shopify's Customer Account API authorization server\n    (issuer https://shopify.com/authentication/47328854173). Storefront browsing and the\n    Storefront MCP server are unauthenticated; authenticated customer operations use OAuth\n    2.0 authorization code + PKCE with OpenID Connect.\nschemes:\n- name: shopify-customer-account-oauth2\n  type: oauth2\n  issuer: https://shopify.com/authentication/47328854173\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/47328854173/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/47328854173/oauth/token\n    endSessionUrl: https://shopify.com/authentication/47328854173/logout\n    codeChallengeMethods:\
  \ [S256]\n    grantTypes: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    tokenEndpointAuthMethods: [client_secret_basic]\n  sources: [well-known/holy-openid-configuration.json]\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://de.holy.com/.well-known/openid-configuration\n  idTokenSigningAlg: [RS256]\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  sources: [well-known/holy-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holy/refs/heads/main/authentication/holy-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Consumer
- Beverages
- Direct-to-Consumer
- Ecommerce
- Agentic Commerce
- Shopify
- Germany
---
