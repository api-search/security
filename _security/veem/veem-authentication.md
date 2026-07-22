---
api_key_in: []
api_specs:
- filename: veem-api-openapi.yml
  format: yaml
  label: Veem Public API
  slug: veem-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-api-openapi.yml
auth_types:
- oauth2
description: Veem Public API authentication profile, captured from the developer-portal OAuth guide (the published OpenAPI operation slices declare no securitySchemes, so this profile is documentation-sourced). Veem uses OAuth 2.0 in two-legged (client_credentials, server-to-server on your own behalf) and three-legged (authorization_code, on behalf of another Veem user) forms, plus refresh_token. Client credentials are sent as an HTTP Basic header (base64 of client_id:client_secret) on the token call; API calls carry the access token as a Bearer Authorization header. Client ID/Secret are generated in the dashboard under Settings > Integrations > Connect Veem API (production credentials are visible only to the primary account owner).
kind: authentication
layout: security
method: searched
name: Veem Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- refreshToken
overview: Veem secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, and refreshToken flow(s).
provider_name: Veem
provider_slug: veem
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    notes: 'Body x-www-form-urlencoded: grant_type=client_credentials, scope=all; Authorization: Basic <base64 client_id:client_secret>. Token response includes access_token, refresh_token, expires_in (~31535999s), account_id, user_id.'
    sandboxTokenUrl: https://sandbox-api.veem.com/oauth/token
    scopes:
    - all
    tokenUrl: https://api.veem.com/oauth/token
  - authorizationUrl: https://api.veem.com/oauth/authorize
    flow: authorizationCode
    notes: '"Connect with Veem" flow; redirect_uri must match one registered with your development keys; response_type=code, then exchange the code at the token endpoint.'
    sandboxAuthorizationUrl: https://sandbox-api.veem.com/oauth/authorize
    sandboxTokenUrl: https://sandbox-api.veem.com/oauth/token
    scopes:
    - all
    tokenUrl: https://api.veem.com/oauth/token
  - flow: refreshToken
    notes: grant_type=refresh_token with the refresh token; expired tokens return 401 Unauthorized.
    tokenUrl: https://api.veem.com/oauth/token
  name: OAuth2
  type: oauth2
slug: veem-authentication
source_filename: veem-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.veem.com/docs/oauth\ndocs: https://developer.veem.com/docs/oauth\ndescription: >-\n  Veem Public API authentication profile, captured from the developer-portal\n  OAuth guide (the published OpenAPI operation slices declare no\n  securitySchemes, so this profile is documentation-sourced). Veem uses OAuth\n  2.0 in two-legged (client_credentials, server-to-server on your own behalf)\n  and three-legged (authorization_code, on behalf of another Veem user) forms,\n  plus refresh_token. Client credentials are sent as an HTTP Basic header\n  (base64 of client_id:client_secret) on the token call; API calls carry the\n  access token as a Bearer Authorization header. Client ID/Secret are generated\n  in the dashboard under Settings > Integrations > Connect Veem API (production\n  credentials are visible only to the primary account owner).\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials, authorizationCode,\
  \ refreshToken]\n  token_style: bearer\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.veem.com/oauth/token\n        sandboxTokenUrl: https://sandbox-api.veem.com/oauth/token\n        scopes: [all]\n        notes: 'Body x-www-form-urlencoded: grant_type=client_credentials, scope=all; Authorization: Basic <base64 client_id:client_secret>. Token response includes access_token, refresh_token, expires_in (~31535999s), account_id, user_id.'\n      - flow: authorizationCode\n        authorizationUrl: https://api.veem.com/oauth/authorize\n        tokenUrl: https://api.veem.com/oauth/token\n        sandboxAuthorizationUrl: https://sandbox-api.veem.com/oauth/authorize\n        sandboxTokenUrl: https://sandbox-api.veem.com/oauth/token\n        scopes: [all]\n        notes: '\"Connect with Veem\" flow; redirect_uri must match one registered with your development keys; response_type=code, then exchange the code at the token\
  \ endpoint.'\n      - flow: refreshToken\n        tokenUrl: https://api.veem.com/oauth/token\n        notes: grant_type=refresh_token with the refresh token; expired tokens return 401 Unauthorized.\nusage:\n  header: 'Authorization: Bearer <access_token>'\n  additional_required_headers:\n    - name: X-Request-Id\n      description: Unique UUID per request; reusing a value returns 409 Conflict (duplicate-request protection). See conventions/veem-conventions.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/authentication/veem-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Payments
- B2B Payments
- Cross-Border Payments
- Invoicing
- Wallets
- Fintech
- Global Payments
---
