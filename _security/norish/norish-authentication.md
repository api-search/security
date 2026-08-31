---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Norish Authentication
name_suffix: Authentication
oauth_flows: []
overview: Norish declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Norish
provider_slug: norish
scheme_count: 0
schemes: []
slug: norish-authentication
source_filename: norish-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Norish Authentication\ngenerated: '2026-08-27'\nmethod: searched\nsource: https://docs.norish.dev/reference/api\ndocs:\n- https://docs.norish.dev/reference/api\n- https://docs.norish.dev/configuration/authentication\nnote: >-\n  Two distinct authentication surfaces exist and should not be confused. (1) The /api/v1 machine API\n  authenticates with an instance-issued API key. (2) Human sign-in to the web app — and therefore to\n  the /api/docs reference and the /api/openapi.json document, which are session-gated — uses Better\n  Auth with email/password, OIDC, GitHub or Google, configured by the instance operator. Norish is\n  self-hosted, so the OIDC/OAuth provider is the operator's own, not a Norish-run identity service.\napi_security_schemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Instance-issued API key sent in the x-api-key request header.\n  source: https://docs.norish.dev/reference/api\n- name: BearerAuth\n  type:\
  \ http\n  scheme: bearer\n  parameter: Authorization\n  description: \"The same instance-issued API key sent as an Authorization header with the Bearer scheme.\"\n  source: https://docs.norish.dev/reference/api\nunauthenticated_operations:\n- method: GET\n  path: /api/v1/health\n  note: >-\n    Public health check. Returns 200 only when both the API and the internal parser service are\n    healthy; it is the endpoint the published docker-compose healthcheck calls.\ngated_surfaces:\n- path: /api/openapi.json\n  gate: signed-in web session\n  note: The generated OpenAPI document is served only to a signed-in user, so it is not publicly fetchable.\n- path: /api/docs\n  gate: signed-in web session\n  note: Scalar API reference; redirects to /login with a callbackUrl when there is no session.\nuser_authentication:\n  framework: Better Auth\n  providers:\n  - id: password\n    name: Email and password\n    default: true\n    note: Enabled automatically when no other provider is configured; PASSWORD_AUTH_ENABLED\
  \ forces it on or off.\n  - id: oidc\n    name: OpenID Connect\n    callback: https://{auth-url-host}/api/auth/oauth2/callback/oidc\n    config:\n    - OIDC_NAME\n    - OIDC_ISSUER\n    - OIDC_CLIENT_ID\n    - OIDC_CLIENT_SECRET\n    - OIDC_WELLKNOWN\n    claim_mapping:\n      enabled_by: OIDC_CLAIM_MAPPING_ENABLED\n      groups_claim_default: groups\n      admin_group_default: norish_admin\n      household_group_prefix_default: norish_household_\n  - id: github\n    name: GitHub OAuth\n    callback: https://{auth-url-host}/api/auth/callback/github\n    config:\n    - GITHUB_CLIENT_ID\n    - GITHUB_CLIENT_SECRET\n  - id: google\n    name: Google OAuth\n    callback: https://{auth-url-host}/api/auth/callback/google\n    config:\n    - GOOGLE_CLIENT_ID\n    - GOOGLE_CLIENT_SECRET\n  bootstrap:\n    first_user_becomes: server owner and server admin\n    registration_after_first_signin: disabled automatically (ENABLE_REGISTRATION default false)\n  brute_force_protection:\n    enabled_by: AUTH_RATE_LIMIT_ENABLED\n\
  \    default: true\n    window_seconds: 60\n    max_requests: 20\nsecrets_handling:\n  master_key: >-\n    MASTER_KEY (32+ characters, `openssl rand -base64 32`) derives the encryption keys protecting\n    stored secrets; changing it invalidates previously encrypted data.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/norish/refs/heads/main/authentication/norish-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Recipes
- Meal Planning
- Groceries
- Food
- Self-Hosted
- Open-Source
- Household
- Calendar
- CalDAV
---
