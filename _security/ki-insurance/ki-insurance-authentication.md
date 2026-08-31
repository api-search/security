---
api_key_in: []
api_specs:
- filename: ki-insurance-administration-api-openapi.yml
  format: yaml
  label: Ki Insurance Administration API
  slug: ki-insurance-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-administration-api-openapi.yml
- filename: ki-insurance-broking-houses-api-openapi.yml
  format: yaml
  label: Ki Insurance Broking Houses API
  slug: ki-insurance-broking-houses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-broking-houses-api-openapi.yml
- filename: ki-insurance-classes-of-business-api-openapi.yml
  format: yaml
  label: Ki Insurance Classes of Business API
  slug: ki-insurance-classes-of-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-classes-of-business-api-openapi.yml
- filename: ki-insurance-configuration-api-openapi.yml
  format: yaml
  label: Ki Insurance Configuration API
  slug: ki-insurance-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-configuration-api-openapi.yml
- filename: ki-insurance-dashboard-api-openapi.yml
  format: yaml
  label: Ki Insurance Dashboard API
  slug: ki-insurance-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-dashboard-api-openapi.yml
- filename: ki-insurance-facilities-api-openapi.yml
  format: yaml
  label: Ki Insurance Facilities API
  slug: ki-insurance-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-facilities-api-openapi.yml
- filename: ki-insurance-indications-api-openapi.yml
  format: yaml
  label: Ki Insurance Indications API
  slug: ki-insurance-indications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-indications-api-openapi.yml
- filename: ki-insurance-leads-api-openapi.yml
  format: yaml
  label: Ki Insurance Leads API
  slug: ki-insurance-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-leads-api-openapi.yml
- filename: ki-insurance-market-leaders-api-openapi.yml
  format: yaml
  label: Ki Insurance Market Leaders API
  slug: ki-insurance-market-leaders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-market-leaders-api-openapi.yml
- filename: ki-insurance-master-data-api-openapi.yml
  format: yaml
  label: Ki Insurance Master Data API
  slug: ki-insurance-master-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-master-data-api-openapi.yml
- filename: ki-insurance-pipeline-api-openapi.yml
  format: yaml
  label: Ki Insurance Pipeline API
  slug: ki-insurance-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-pipeline-api-openapi.yml
- filename: ki-insurance-quotes-api-openapi.yml
  format: yaml
  label: Ki Insurance Quotes API
  slug: ki-insurance-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-quotes-api-openapi.yml
- filename: ki-insurance-risk-codes-api-openapi.yml
  format: yaml
  label: Ki Insurance Risk Codes API
  slug: ki-insurance-risk-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-risk-codes-api-openapi.yml
- filename: ki-insurance-schedule-of-values-api-openapi.yml
  format: yaml
  label: Ki Insurance Schedule of Values API
  slug: ki-insurance-schedule-of-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-schedule-of-values-api-openapi.yml
- filename: ki-insurance-slip-extraction-api-openapi.yml
  format: yaml
  label: Ki Insurance Slip Extraction API
  slug: ki-insurance-slip-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-slip-extraction-api-openapi.yml
- filename: ki-insurance-support-api-openapi.yml
  format: yaml
  label: Ki Insurance Support API
  slug: ki-insurance-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-support-api-openapi.yml
- filename: ki-insurance-telemetry-api-openapi.yml
  format: yaml
  label: Ki Insurance Telemetry API
  slug: ki-insurance-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-telemetry-api-openapi.yml
- filename: ki-insurance-users-api-openapi.yml
  format: yaml
  label: Ki Insurance Users API
  slug: ki-insurance-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-users-api-openapi.yml
auth_types:
- http
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ki Insurance Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Ki Insurance secures its APIs with http, openIdConnect, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Ki Insurance
provider_slug: ki-insurance
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: 'Auth0-issued access token. Observed in the platform client''s request helper, which sets `Authorization: Bearer <token>`, `Accept: application/json` and `Content-Type: application/json` on every request and uses `credentials: same-origin`.'
  name: auth0Bearer
  scheme: bearer
  sources:
  - openapi/ki-insurance-broker-platform-openapi.yml
  - https://app.ki-insurance.com/assets/index-DgeF7w2c.js
  type: http
- description: Auth0 OIDC discovery for the partner login.
  name: auth0OpenId
  openIdConnectUrl: https://login.ki-insurance.com/.well-known/openid-configuration
  sources:
  - openapi/ki-insurance-broker-platform-openapi.yml
  type: openIdConnect
- description: The underlying Auth0 authorization server. Flow values below are read verbatim from the anonymous discovery document; Ki publishes no business scopes.
  flows:
  - authorizationUrl: https://login.ki-insurance.com/authorize
    flow: authorizationCode
    refreshUrl: https://login.ki-insurance.com/oauth/token
    tokenUrl: https://login.ki-insurance.com/oauth/token
  name: auth0OAuth2
  sources:
  - https://login.ki-insurance.com/.well-known/openid-configuration
  type: oauth2
slug: ki-insurance-authentication
source_filename: ki-insurance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://login.ki-insurance.com/.well-known/openid-configuration\ndocs: https://login.ki-insurance.com/.well-known/openid-configuration\nderived_from:\n- openapi/ki-insurance-broker-platform-openapi.yml\n- https://app.ki-insurance.com/config.js\nsummary:\n  types:\n  - http\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  model: >-\n    Partner-gated OAuth 2.0 / OpenID Connect. Ki fronts an Auth0 EU tenant at\n    login.ki-insurance.com. The broker single-page app performs an\n    authorization-code + PKCE login and then attaches the resulting Auth0 access\n    token as `Authorization: Bearer <JWT>` to every call against the same-origin\n    /api surface on app.ki-insurance.com. There is no API key, no mTLS scheme and\n    no self-serve credential issuance published anywhere on Ki's public surface.\nschemes:\n- name: auth0Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n\
  \  description: >-\n    Auth0-issued access token. Observed in the platform client's request helper,\n    which sets `Authorization: Bearer <token>`, `Accept: application/json` and\n    `Content-Type: application/json` on every request and uses\n    `credentials: same-origin`.\n  sources:\n  - openapi/ki-insurance-broker-platform-openapi.yml\n  - https://app.ki-insurance.com/assets/index-DgeF7w2c.js\n- name: auth0OpenId\n  type: openIdConnect\n  openIdConnectUrl: https://login.ki-insurance.com/.well-known/openid-configuration\n  description: Auth0 OIDC discovery for the partner login.\n  sources:\n  - openapi/ki-insurance-broker-platform-openapi.yml\n- name: auth0OAuth2\n  type: oauth2\n  description: >-\n    The underlying Auth0 authorization server. Flow values below are read verbatim\n    from the anonymous discovery document; Ki publishes no business scopes.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.ki-insurance.com/authorize\n    tokenUrl: https://login.ki-insurance.com/oauth/token\n\
  \    refreshUrl: https://login.ki-insurance.com/oauth/token\n  sources:\n  - https://login.ki-insurance.com/.well-known/openid-configuration\nissuer:\n  issuer: https://login.ki-insurance.com/\n  audience: https://api.ki.com\n  audience_note: >-\n    The audience string is published in the platform runtime config at\n    https://app.ki-insurance.com/config.js. It is an identifier, not a reachable\n    host — api.ki.com resolves to a parked \"Site Not Configured\" page.\n  tenant: Auth0 (EU region, ki-prod)\n  endpoints:\n    authorization: https://login.ki-insurance.com/authorize\n    token: https://login.ki-insurance.com/oauth/token\n    userinfo: https://login.ki-insurance.com/userinfo\n    jwks: https://login.ki-insurance.com/.well-known/jwks.json\n    revocation: https://login.ki-insurance.com/oauth/revoke\n    device_authorization: https://login.ki-insurance.com/oauth/device/code\n    dynamic_client_registration: https://login.ki-insurance.com/oidc/register\n    mfa_challenge: https://login.ki-insurance.com/mfa/challenge\n\
  \    global_token_revocation: https://login.ki-insurance.com/oauth/global-token-revocation/connection/{connectionName}\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  code_challenge_methods_supported:\n  - S256\n  - plain\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  id_token_signing_alg_values_supported:\n  - HS256\n  - RS256\n  - PS256\n  response_modes_supported:\n  - query\n  - fragment\n  - form_post\n  backchannel_logout_supported: true\n  mfa: >-\n    The tenant advertises MFA grant types (mfa-oob, mfa-otp, mfa-recovery-code)\n    and an /mfa/challenge endpoint; Ki does not document whether partner brokers\n    are enrolled.\nlogin_flow:\n  entry: https://auth.ki-insurance.com/login?return_to=<url>\n\
  \  note: >-\n    Ki runs its own thin login/logout shim at auth.ki-insurance.com in front of\n    Auth0. GET /login without return_to responds `Missing 'return_to' query\n    parameter.` (HTTP 400); GET /logout (HTTP 302) redirects to\n    https://login.ki-insurance.com/v2/logout. The shim is not an OIDC issuer —\n    its /.well-known/openid-configuration is 404.\n  callback: https://app.ki-insurance.com/auth/callback\ngaps:\n- No published scope model for the Ki API itself (see scopes/ki-insurance-scopes.yml).\n- No API-key, mTLS, signed-request or partner-SAML scheme is documented publicly.\n- No self-serve credential issuance; access is granted per partner broking house.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/authentication/ki-insurance-authentication.yml
summary_line: http/openIdConnect/oauth2 · 3 schemes
tags:
- Insurance
- United Kingdom
- Lloyd's of London
- Specialty Insurance
- Property and Casualty
- Underwriting
- Insurtech
- Brokers
- Algorithmic Underwriting
- Reinsurance
---
