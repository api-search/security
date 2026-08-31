---
api_key_in:
- header
api_specs:
- filename: onpay-company-api-openapi.yml
  format: yaml
  label: OnPay Company API
  slug: onpay-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onpay/refs/heads/main/openapi/onpay-company-api-openapi.yml
- filename: onpay-deductions-api-openapi.yml
  format: yaml
  label: OnPay Deductions API
  slug: onpay-deductions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onpay/refs/heads/main/openapi/onpay-deductions-api-openapi.yml
- filename: onpay-employees-api-openapi.yml
  format: yaml
  label: OnPay Employees API
  slug: onpay-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onpay/refs/heads/main/openapi/onpay-employees-api-openapi.yml
- filename: onpay-pay-runs-api-openapi.yml
  format: yaml
  label: OnPay Pay Runs API
  slug: onpay-pay-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onpay/refs/heads/main/openapi/onpay-pay-runs-api-openapi.yml
- filename: onpay-reports-api-openapi.yml
  format: yaml
  label: OnPay Reports API
  slug: onpay-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onpay/refs/heads/main/openapi/onpay-reports-api-openapi.yml
- filename: onpay-user-api-openapi.yml
  format: yaml
  label: OnPay User API
  slug: onpay-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onpay/refs/heads/main/openapi/onpay-user-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Onpay Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: OnPay secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: OnPay
provider_slug: onpay
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://app.onpay.com/app/oauth/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://app.onpay.com/app/oauth/authorize
    tokenUrl_documented: https://app.onpay.com/app/oauth/token
    tokenUrl_note: The published OpenAPI sets tokenUrl identical to authorizationUrl. The authorization guide documents the token endpoint as /app/oauth/token. The spec value is wrong and will break any generated client; captured as a correction in overlays/onpay-api-overlay.yaml.
  name: OAuth2
  sources:
  - openapi/onpay-api-openapi.json
  type: oauth2
- format: Bearer {access_token}
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/onpay-api-openapi.json
  type: apiKey
slug: onpay-authentication
source_filename: onpay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: openapi/onpay-api-openapi.json\ndocs: https://onpay.readme.io/reference/authorization\naccess:\n  model: partner-only\n  self_serve: false\n  quoted: 'The OnPay API has access limited to approved partners only. To partner, please contact us.'\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.onpay.com/app/oauth/authorize\n    tokenUrl: https://app.onpay.com/app/oauth/authorize\n    tokenUrl_documented: https://app.onpay.com/app/oauth/token\n    tokenUrl_note: >-\n      The published OpenAPI sets tokenUrl identical to authorizationUrl. The authorization guide\n      documents the token endpoint as /app/oauth/token. The spec value is wrong and will break any\n      generated client; captured as a correction in overlays/onpay-api-overlay.yaml.\n    scopes:\
  \ 6\n  sources:\n  - openapi/onpay-api-openapi.json\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer {access_token}'\n  sources:\n  - openapi/onpay-api-openapi.json\nflow:\n  grant: authorization_code\n  steps:\n  - Redirect the user to /app/oauth/authorize with client_id, redirect_uri and state.\n  - The user approves access to their OnPay company.\n  - OnPay redirects back to redirect_uri with an authorization code.\n  - Server-side POST to /app/oauth/token (application/x-www-form-urlencoded) with client_id,\n    client_secret, redirect_uri, code and grant_type=authorization_code.\n  - Send Authorization \"Bearer {access_token}\" on every API request.\n  - Exchange the refresh token for a new access/refresh pair with grant_type=refresh_token.\n  token:\n    type: bearer\n    lifetime_seconds: 7200\n    response_fields: [access_token, token_type, expires_in, refresh_token, company_id, access_type,\n      company_name]\n    company_scoped: true\n\
  \    note: >-\n      The token response carries company_id and company_name — one token authorizes exactly one OnPay\n      company, and access_type carries the numeric role (see scopes/onpay-scopes.yml).\n  refresh_token:\n    single_use: true\n    note: >-\n      \"You can exchange your refresh token for a new access token, only once.\" Each exchange returns a\n      NEW refresh token; failing to persist it loses the connection.\n  failure: >-\n    The docs state that a missing or expired access token results in a 401. Observed live, a request\n    with no Authorization header returns HTTP 400 with error_code 100 \"Missing token\"; an invalid\n    bearer token can return 401 or 403 with \"expired token\".\ngaps:\n- No OAuth 2.0 Authorization Server Metadata (RFC 8414) — /.well-known/oauth-authorization-server 404s.\n- No OpenID Connect discovery document.\n- No PKCE guidance, and no documented state/nonce requirements beyond the example link.\n- No token-revocation or introspection endpoint\
  \ is published.\n- No mTLS, no API-key alternative, and no service-to-service credential for backend integrations.\n- The authorization guide still instructs partners to send client_id, client_secret and authorization\n  codes to onpaydev.com, a domain that is now parked (see sandbox/onpay-sandbox.yml).\nx-evidence:\n- url: https://onpay.readme.io/reference/authorization.md\n  http_status: 200\n  fetched: '2026-08-04'\n- url: https://app.onpay.com/app/oauth/authorize\n  http_status: 302\n  fetched: '2026-08-04'\n- url: https://api.onpay.com/v2/employees\n  http_status: 400\n  fetched: '2026-08-04'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onpay/refs/heads/main/authentication/onpay-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- payroll
- human-resources
- employee-benefits
- payroll-tax
- small-business
- workforce-management
- Fintech
- hr-tech
- time-and-attendance
- retirement-401k
---
