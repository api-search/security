---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Paystand Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- password
overview: PayStand secures its APIs with oauth2, apiKey, and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, and password flow(s).
provider_name: PayStand
provider_slug: paystand
scheme_count: 4
schemes:
- flows:
  - flow: clientCredentials
    scopes:
    - auth
    tokenUrl: https://api.paystand.com/v3/api/v3/oauth/token
  - authorizationUrl: https://api.paystand.com/v3/api/v3/oauth/authorize
    flow: authorizationCode
    scopes:
    - auth
    tokenUrl: https://api.paystand.com/v3/api/v3/oauth/token
  name: oauth2
  source: https://api.paystand.com/.well-known/openid-configuration
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
- description: Bearer <access_token> for authenticated calls.
  name: Authorization
  scheme: bearer
  source: https://developers.paystand.com/reference/headers
  type: http
- description: Customer id, required for authenticated calls.
  in: header
  name: X-CUSTOMER-ID
  parameter: X-CUSTOMER-ID
  source: https://developers.paystand.com/reference/headers
  type: apiKey
- description: Customer's publishable API key, required for non-authenticated (public) calls.
  in: header
  name: X-PUBLISHABLE-KEY
  parameter: X-PUBLISHABLE-KEY
  source: https://developers.paystand.com/reference/headers
  type: apiKey
slug: paystand-authentication
source_filename: paystand-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.paystand.com/.well-known/openid-configuration\ndocs: https://developers.paystand.com/reference/getting-api-access\nsummary:\n  types: [oauth2, apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials, authorizationCode, password]\nnotes: >-\n  Authenticated Paystand API calls use an OAuth2 access token in the\n  Authorization header (\"Bearer <token>\") plus an X-CUSTOMER-ID header. Access\n  tokens are minted at the token endpoint with grant_type=client_credentials\n  using the application clientId/clientSecret (scope \"auth\"). Non-authenticated\n  (public checkout) calls use the X-PUBLISHABLE-KEY header carrying the\n  customer's publishable key.\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.paystand.com/v3/api/v3/oauth/token\n    scopes: [auth]\n  - flow: authorizationCode\n    authorizationUrl: https://api.paystand.com/v3/api/v3/oauth/authorize\n\
  \    tokenUrl: https://api.paystand.com/v3/api/v3/oauth/token\n    scopes: [auth]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  source: https://api.paystand.com/.well-known/openid-configuration\n- name: Authorization\n  type: http\n  scheme: bearer\n  description: \"Bearer <access_token> for authenticated calls.\"\n  source: https://developers.paystand.com/reference/headers\n- name: X-CUSTOMER-ID\n  type: apiKey\n  in: header\n  parameter: X-CUSTOMER-ID\n  description: Customer id, required for authenticated calls.\n  source: https://developers.paystand.com/reference/headers\n- name: X-PUBLISHABLE-KEY\n  type: apiKey\n  in: header\n  parameter: X-PUBLISHABLE-KEY\n  description: Customer's publishable API key, required for non-authenticated (public) calls.\n  source: https://developers.paystand.com/reference/headers\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paystand/refs/heads/main/authentication/paystand-authentication.yml
summary_line: oauth2/apiKey/http · 4 schemes
tags:
- Company
- Payments
- B2B Payments
- Accounts Receivable
- Accounts Payable
- Fintech
- Blockchain
- ACH
- Billing
- Checkout
---
