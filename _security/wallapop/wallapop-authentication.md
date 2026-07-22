---
api_key_in: []
api_specs:
- filename: wallapop-items-openapi-original.yml
  format: yaml
  label: Wallapop Items Connect API
  slug: wallapop-items-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallapop/refs/heads/main/openapi/wallapop-items-openapi-original.yml
- filename: wallapop-transactions-openapi-original.yml
  format: yaml
  label: Wallapop Transactions Connect API
  slug: wallapop-transactions-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallapop/refs/heads/main/openapi/wallapop-transactions-openapi-original.yml
- filename: wallapop-webhooks-openapi-original.yml
  format: yaml
  label: Wallapop Webhooks Connect API
  slug: wallapop-webhooks-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallapop/refs/heads/main/openapi/wallapop-webhooks-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Wallapop Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wallapop secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wallapop
provider_slug: wallapop
scheme_count: 1
schemes:
- description: The Items Connect API uses OAuth 2.0 Authorization Code flow with a Proof Key for Code Exchange.
  flows:
  - authorizationUrl: https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/auth
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/token
  name: oAuthWithPKCE
  sources:
  - openapi/wallapop-items-openapi-original.yml
  - openapi/wallapop-transactions-openapi-original.yml
  - openapi/wallapop-webhooks-openapi-original.yml
  type: oauth2
slug: wallapop-authentication
source_filename: wallapop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/wallapop-items-openapi-original.yml, openapi/wallapop-transactions-openapi-original.yml,\n  openapi/wallapop-webhooks-openapi-original.yml\ndocs: https://developers.wallapop.com/pages/api-essentials/auth\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: required (S256)\n  token_use: Bearer access token in the Authorization header on every connect.wallapop.com request\nschemes:\n- name: oAuthWithPKCE\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/auth\n    tokenUrl: https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/token\n    scopes: 0\n  description: The Items Connect API uses OAuth 2.0 Authorization Code flow with a Proof Key\n    for Code Exchange.\n  sources:\n  - openapi/wallapop-items-openapi-original.yml\n  - openapi/wallapop-transactions-openapi-original.yml\n\
  \  - openapi/wallapop-webhooks-openapi-original.yml\ndetails:\n  authorization_server: Keycloak realm wallapop-connect at iam.wallapop.com (OIDC discovery captured in well-known/wallapop-openid-configuration.json)\n  credentials: >-\n    One application credential (public client_id + confidential client_secret)\n    per integrator application — not per managed user; user consent produces\n    per-user token pairs.\n  pkce: >-\n    code_verifier is a URL-safe random string of at least 43 characters;\n    code_challenge = BASE64URL-ENCODE(SHA256(ASCII(code_verifier))) with method\n    S256.\n  token_exchange: >-\n    POST to the token endpoint with grant_type=authorization_code, code,\n    redirect_uri, code_verifier, client_id, client_secret. A valid User-Agent\n    header is required or the request may be rejected. Authorization codes are\n    single-use and expire quickly (invalid_grant otherwise).\n  refresh: >-\n    grant_type=refresh_token returns a new access_token AND a new\n   \
  \ refresh_token; the application must store the new refresh token and\n    discard the previous one. Refresh tokens have a maximum lifetime.\n  token_response_scope: offline_access\n  rate_limits: >-\n    Token endpoints are limited to 174 requests per 5 minutes per source IP for\n    both authorization_code and refresh_token grants (see\n    rate-limits/wallapop-rate-limits.yml).\n  state_parameter: >-\n    Docs recommend the state parameter to correlate callbacks to users and\n    prevent CSRF.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wallapop/refs/heads/main/authentication/wallapop-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Consumer
- Marketplace
- Ecommerce
- Second-Hand
- Classifieds
- Shipping
- Webhooks
---
