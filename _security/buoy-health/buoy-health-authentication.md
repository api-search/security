---
api_key_in: []
api_specs:
- filename: buoy-health-complaints-api-openapi.yml
  format: yaml
  label: Buoy Health Complaints API
  slug: buoy-health-complaints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-complaints-api-openapi.yml
- filename: buoy-health-intents-api-openapi.yml
  format: yaml
  label: Buoy Health Intents API
  slug: buoy-health-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-intents-api-openapi.yml
- filename: buoy-health-interviews-api-openapi.yml
  format: yaml
  label: Buoy Health Interviews API
  slug: buoy-health-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-interviews-api-openapi.yml
- filename: buoy-health-queries-api-openapi.yml
  format: yaml
  label: Buoy Health Queries API
  slug: buoy-health-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-queries-api-openapi.yml
- filename: buoy-health-questions-api-openapi.yml
  format: yaml
  label: Buoy Health Questions API
  slug: buoy-health-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-questions-api-openapi.yml
- filename: buoy-health-results-api-openapi.yml
  format: yaml
  label: Buoy Health Results API
  slug: buoy-health-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-results-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Buoy Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Buoy Health secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Buoy Health
provider_slug: buoy-health
scheme_count: 1
schemes:
- applied: global
  description: '[Full documentation for the Buoy Auth API is found here.](https://sandbox.buoyhealth.com/auth/redoc/)'
  flows:
  - authorizationUrl: https://auth.sandbox.buoyhealth.com/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://auth.sandbox.buoyhealth.com/oauth/token
  name: Bearer
  sources:
  - openapi/buoy-health-symptom-checker-openapi.yml
  type: oauth2
slug: buoy-health-authentication
source_filename: buoy-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: searched\nsource: openapi/buoy-health-symptom-checker-openapi.yml\ndocs: https://auth.buoyhealth.com/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  api_key_in: []\n  bearer_only: true\n  scope_flat: true\n  note: >-\n    Every one of the 19 operations in the Symptom Checker OpenAPI inherits the single global\n    `security: [{Bearer: []}]` requirement, and every operation documents a 401 response. There is no\n    API-key alternative and no per-operation scope differentiation.\nschemes:\n- name: Bearer\n  type: oauth2\n  applied: global\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.sandbox.buoyhealth.com/authorize\n    tokenUrl: https://auth.sandbox.buoyhealth.com/oauth/token\n    scopes: 0\n  description: '[Full documentation for the Buoy Auth API is found here.](https://sandbox.buoyhealth.com/auth/redoc/)'\n  sources:\n  - openapi/buoy-health-symptom-checker-openapi.yml\n\
  authorization_servers:\n- environment: production\n  issuer: https://auth.buoyhealth.com/\n  authorization_endpoint: https://auth.buoyhealth.com/authorize\n  token_endpoint: https://auth.buoyhealth.com/oauth/token\n  userinfo_endpoint: https://auth.buoyhealth.com/userinfo\n  jwks_uri: https://auth.buoyhealth.com/.well-known/jwks.json\n  revocation_endpoint: https://auth.buoyhealth.com/oauth/revoke\n  registration_endpoint: https://auth.buoyhealth.com/oidc/register\n  device_authorization_endpoint: https://auth.buoyhealth.com/oauth/device/code\n  discovery:\n  - well-known/buoy-health-openid-configuration.json\n  - well-known/buoy-health-oauth-authorization-server.json\n  platform: Auth0\n- environment: sandbox\n  issuer: https://auth.sandbox.buoyhealth.com/\n  authorization_endpoint: https://auth.sandbox.buoyhealth.com/authorize\n  token_endpoint: https://auth.sandbox.buoyhealth.com/oauth/token\n  userinfo_endpoint: https://auth.sandbox.buoyhealth.com/userinfo\n  jwks_uri: https://auth.sandbox.buoyhealth.com/.well-known/jwks.json\n\
  \  revocation_endpoint: https://auth.sandbox.buoyhealth.com/oauth/revoke\n  registration_endpoint: https://auth.sandbox.buoyhealth.com/oidc/register\n  device_authorization_endpoint: https://auth.sandbox.buoyhealth.com/oauth/device/code\n  discovery:\n  - well-known/buoy-health-sandbox-openid-configuration.json\n  - well-known/buoy-health-sandbox-oauth-authorization-server.json\n  platform: Auth0\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\n- password\n- implicit\n- 'urn:ietf:params:oauth:grant-type:device_code'\n- 'urn:ietf:params:oauth:grant-type:token-exchange'\n- 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n- 'http://auth0.com/oauth/grant-type/password-realm'\n- 'http://auth0.com/oauth/grant-type/passwordless/otp'\n- 'http://auth0.com/oauth/grant-type/mfa-oob'\n- 'http://auth0.com/oauth/grant-type/mfa-otp'\n- 'http://auth0.com/oauth/grant-type/mfa-recovery-code'\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n\
  - private_key_jwt\n- none\npkce:\n  supported: true\n  code_challenge_methods: [S256, plain]\nid_token_signing_alg_values_supported: [HS256, RS256, PS256]\nmfa:\n  challenge_endpoint: https://auth.buoyhealth.com/mfa/challenge\n  grant_types: [mfa-oob, mfa-otp, mfa-recovery-code]\nobservations:\n- id: spec-points-at-sandbox-only\n  detail: >-\n    The OpenAPI's oauth2 flow hardcodes the SANDBOX authorization and token endpoints\n    (auth.sandbox.buoyhealth.com) while listing both the sandbox and production API servers. A client\n    generated straight from the spec will authenticate against sandbox even when calling production.\n    The production issuer (auth.buoyhealth.com) is only discoverable by probing /.well-known/.\n- id: empty-scopes-map\n  detail: >-\n    The oauth2 scheme declares an empty `scopes` map and no operation names a scope, so the spec\n    conveys no least-privilege model — a token is all-or-nothing across the whole triage surface.\n- id: plain-pkce-allowed\n  detail:\
  \ >-\n    The authorization server advertises `plain` alongside `S256` in code_challenge_methods_supported.\n- id: no-protected-resource-metadata\n  detail: >-\n    Neither API host publishes RFC 9728 oauth-protected-resource metadata, so the resource-to-issuer\n    binding cannot be discovered mechanically.\nx-evidence:\n- url: https://auth.buoyhealth.com/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-08-08'\n- url: https://auth.sandbox.buoyhealth.com/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-08'\n- url: https://sandbox.buoyhealth.com/auth/redoc/\n  http_status: 401\n  fetched: '2026-08-08'\n  note: The Buoy Auth API reference the OpenAPI links to is itself credential-gated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/authentication/buoy-health-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Symptom Checker
- medical-triage
- Digital Health
- Healthcare
- Clinical AI
- Care Navigation
- Patient Engagement
- Diagnosis
- Telehealth
- Authentication
---
