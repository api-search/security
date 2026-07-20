---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Flipkart Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Flipkart secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Flipkart
provider_slug: flipkart
scheme_count: 1
schemes:
- client_authentication: HTTP Basic (Base64 appId:appSecret)
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.flipkart.net/oauth-service/oauth/token
    usage: self-access applications
  - authorizationUrl: https://api.flipkart.net/oauth-service/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.flipkart.net/oauth-service/oauth/token
    usage: third-party applications acting on behalf of sellers
  name: OAuth2
  scopes:
  - Seller_Api
  - Default
  token_expiry:
    access_token_days: 60
    expiry_check: https://api.flipkart.net/oauth-service/oauth/token/expiry
    refresh_token_days: 180
  type: oauth2
slug: flipkart-authentication
source_filename: flipkart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://seller.flipkart.com/api-docs/FMSAPI.html\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  notes: >-\n    Flipkart Marketplace Seller API v3 is protected with OAuth 2.0. Self-access applications use the\n    client-credentials grant; third-party applications that act on behalf of many sellers use the\n    authorization-code grant. The token endpoint requires HTTP Basic authentication with a\n    Base64-encoded appId:appSecret. Access tokens are valid for ~60 days and refresh tokens for ~180\n    days; expiry can be checked via the oauth-service token/expiry endpoint. Expired tokens return HTTP\n    401.\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.flipkart.net/oauth-service/oauth/token\n    usage: self-access applications\n  - flow: authorizationCode\n    authorizationUrl: https://api.flipkart.net/oauth-service/oauth/authorize\n\
  \    tokenUrl: https://api.flipkart.net/oauth-service/oauth/token\n    usage: third-party applications acting on behalf of sellers\n  client_authentication: HTTP Basic (Base64 appId:appSecret)\n  token_expiry:\n    access_token_days: 60\n    refresh_token_days: 180\n    expiry_check: https://api.flipkart.net/oauth-service/oauth/token/expiry\n  scopes:\n  - Seller_Api\n  - Default\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flipkart/refs/heads/main/authentication/flipkart-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Consumer
- E-Commerce
- Marketplace
- Retail
- Sellers
- Orders
- Fulfillment
- India
- OAuth
---
