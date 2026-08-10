---
api_key_in: []
api_specs:
- filename: nursa-clinicians-api-openapi.yml
  format: yaml
  label: Nursa Clinicians API
  slug: nursa-clinicians-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-clinicians-api-openapi.yml
- filename: nursa-downloads-api-openapi.yml
  format: yaml
  label: Nursa Downloads API
  slug: nursa-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-downloads-api-openapi.yml
- filename: nursa-facilities-api-openapi.yml
  format: yaml
  label: Nursa Facilities API
  slug: nursa-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-facilities-api-openapi.yml
- filename: nursa-facilities-webhooks-api-openapi.yml
  format: yaml
  label: Nursa Facilities webhooks API
  slug: nursa-facilities-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-facilities-webhooks-api-openapi.yml
- filename: nursa-licenses-api-openapi.yml
  format: yaml
  label: Nursa Licenses API
  slug: nursa-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-licenses-api-openapi.yml
- filename: nursa-marketplace-api-openapi.yml
  format: yaml
  label: Nursa Marketplace API
  slug: nursa-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-marketplace-api-openapi.yml
- filename: nursa-scheduled-shifts-api-openapi.yml
  format: yaml
  label: Nursa Scheduled shifts API
  slug: nursa-scheduled-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-scheduled-shifts-api-openapi.yml
- filename: nursa-shift-reports-api-openapi.yml
  format: yaml
  label: Nursa Shift reports API
  slug: nursa-shift-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-shift-reports-api-openapi.yml
- filename: nursa-shift-requests-api-openapi.yml
  format: yaml
  label: Nursa Shift requests API
  slug: nursa-shift-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-shift-requests-api-openapi.yml
- filename: nursa-shifts-api-openapi.yml
  format: yaml
  label: Nursa Shifts API
  slug: nursa-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-shifts-api-openapi.yml
- filename: nursa-support-api-openapi.yml
  format: yaml
  label: Nursa Support API
  slug: nursa-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-support-api-openapi.yml
- filename: nursa-user-webhooks-api-openapi.yml
  format: yaml
  label: Nursa User webhooks API
  slug: nursa-user-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-user-webhooks-api-openapi.yml
- filename: nursa-webhook-logs-api-openapi.yml
  format: yaml
  label: Nursa Webhook logs API
  slug: nursa-webhook-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-webhook-logs-api-openapi.yml
auth_types:
- http
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nursa Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- authorizationCode+PKCE
- password
- implicit
- clientCredentials
- refreshToken
overview: Nursa secures its APIs with http, openIdConnect, and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, authorizationCode+PKCE, password, implicit, clientCredentials, and refreshToken flow(s).
provider_name: Nursa
provider_slug: nursa
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Please, fill this with your authorization token
  name: public-api
  scheme: bearer
  sources:
  - openapi/nursa-public-api-v2-openapi.yml
  type: http
- description: Nursa Authorization Server. Not declared in the OpenAPI; documented at docs.nursa.com/docs/Integration Guideline/Authentication and confirmed by a live 200 on the discovery document.
  name: nursa-oidc
  openIdConnectUrl: https://auth.nursa.com/oidc/.well-known/openid-configuration
  sources:
  - https://docs.nursa.com/docs/Integration%20Guideline/Authentication/
  - well-known/nursa-openid-configuration.json
  type: openIdConnect
slug: nursa-authentication
source_filename: nursa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: openapi/nursa-public-api-v2-openapi.yml\ndocs: https://docs.nursa.com/docs/Integration%20Guideline/Authentication/\nsummary:\n  types:\n  - http\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - authorizationCode+PKCE\n  - password\n  - implicit\n  - clientCredentials\n  - refreshToken\n  note: >-\n    The OpenAPI surface declares only `http bearer` (JWT) — the token itself is minted by a full\n    OpenID Connect / OAuth 2.0 authorization server that the spec never references. The spec has no\n    `openIdConnect` or `oauth2` securityScheme and no `openIdConnectUrl`, so the machine-readable\n    contract understates the real auth model by a wide margin. This file is the reconciled view.\nschemes:\n- name: public-api\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Please, fill this with your authorization token\n  sources:\n  - openapi/nursa-public-api-v2-openapi.yml\n\
  - name: nursa-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://auth.nursa.com/oidc/.well-known/openid-configuration\n  description: >-\n    Nursa Authorization Server. Not declared in the OpenAPI; documented at\n    docs.nursa.com/docs/Integration Guideline/Authentication and confirmed by a live 200 on the\n    discovery document.\n  sources:\n  - https://docs.nursa.com/docs/Integration%20Guideline/Authentication/\n  - well-known/nursa-openid-configuration.json\nenvironments:\n- name: production\n  issuer: https://auth.nursa.com/\n  authorization_endpoint: https://auth.nursa.com/oidc/authorize\n  token_endpoint: https://auth.nursa.com/oidc/oauth/token\n  userinfo_endpoint: https://auth.nursa.com/oidc/userinfo\n  end_session_endpoint: https://auth.nursa.com/oidc/logout\n  jwks_uri: https://auth.nursa.com/oidc/.well-known/jwks.json\n  api_base: https://public-api.prod.nursa.com\n  developer_portal: https://developers.prod.nursa.com/\n- name: sandbox\n  issuer: https://auth.sandbox.nursa.com/\n\
  \  authorization_endpoint: https://auth.sandbox.nursa.com/oidc/authorize\n  token_endpoint: https://auth.sandbox.nursa.com/oidc/oauth/token\n  userinfo_endpoint: https://auth.sandbox.nursa.com/oidc/userinfo\n  end_session_endpoint: https://auth.sandbox.nursa.com/oidc/logout\n  jwks_uri: https://auth.sandbox.nursa.com/oidc/.well-known/jwks.json\n  api_base: https://public-api.sandbox.nursa.com\n  developer_portal: https://developers.sandbox.nursa.com/\n  sign_up: https://nursa-sandbox.web.app/\ngrants:\n- id: authorization_code\n  supported: true\n  recommended_for: regular web applications with a secure back end\n- id: authorization_code_pkce\n  supported: true\n  code_challenge_methods:\n  - S256\n  - plain\n  recommended_for: native, mobile and single-page applications\n- id: client_credentials\n  supported: true\n  gated: true\n  note: >-\n    Machine-to-machine. Nursa enables the client credentials grant on an application only on\n    explicit request, \"due to security reasons\" —\
  \ actions in Nursa must be attributable to a user,\n    so a M2M app has to be associated with a facility user before it can act.\n- id: password\n  supported: true\n  note: Resource Owner Password flow; listed in the docs but discouraged by current OAuth BCP.\n- id: implicit\n  supported: true\n  note: Implicit flow; listed in the docs. Deprecated by OAuth 2.1 / Security BCP (RFC 9700).\n- id: refresh_token\n  supported: true\n  note: requires the offline_access scope\ntokens:\n  format: JWT (RS256)\n  transport: Authorization Bearer header\n  access_token_ttl: 1 hour (production); 24 hours (sandbox, client-credentials)\n  refresh_token: rotating, single-use, 30-day default expiry; non-rotating available on request\n  id_token_claims:\n  - iss\n  - aud\n  - nonce\n  - sid\n  - sub\n  - name\n  - nickname\n  - picture\n  - phone_number\n  - email\n  - role\n  - address\n  - iat\n  - exp\n  access_token_claims:\n  - iss\n  - sub\n  - role\n  - aud\n  - azp\n  - scope\n  - iat\n  - exp\n\
  \  roles:\n  - NURSE_USER\n  - FACILITY_USER\n  id_token_signing_alg_values_supported:\n  - RS256\nenforcement:\n  missing_token: HTTP 401 {\"message\":\"Unauthorized\",\"statusCode\":401}\n  missing_scope: HTTP 403 {\"message\":\"Forbidden Resource\",\"error\":\"Forbidden\",\"statusCode\":403}\ngaps:\n- >-\n  The OpenAPI declares no oauth2/openIdConnect scheme and no per-operation scope requirements, so\n  no scope can be resolved from the machine-readable contract — the scope table lives only in prose\n  at docs.nursa.com/docs/Integration Guideline/Scopes.\n- Implicit and Resource Owner Password grants are still advertised as supported.\n- No mutualTLS, no DPoP / proof-of-possession, no private_key_jwt client authentication documented.\n- >-\n  The discovery document advertises `code_challenge_methods_supported: [S256, plain]`; `plain`\n  weakens PKCE and is discouraged by RFC 7636 and OAuth 2.1.\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - url: https://docs.nursa.com/docs/Integration%20Guideline/Authentication/\n\
  \    status: 200\n  - url: https://auth.nursa.com/oidc/.well-known/openid-configuration\n    status: 200\n  - url: https://auth.sandbox.nursa.com/oidc/.well-known/openid-configuration\n    status: 200\n  - url: https://public-api.prod.nursa.com/api/v2/public/licenses\n    status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/authentication/nursa-authentication.yml
summary_line: http/openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Healthcare
- Health
- Staffing
- Nursing
- Marketplace
- Workforce Management
- Scheduling
- Human Resources
- Per Diem
- Shifts
- Webhooks
---
