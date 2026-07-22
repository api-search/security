---
api_key_in: []
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Zipline Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zipline Ai secures its APIs with http, oauth2, and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zipline Ai
provider_slug: zipline-ai
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Short-lived JWT minted by `zipline auth get-access-token` (or issued to the frontend after OAuth/SSO login). Backend services validate it statelessly against the JWKS endpoint (AUTH_JWKS_URL, e.g. /api/auth/jwks). When AUTH_ENABLED=true but the JWKS endpoint is unreachable, protected routes return 503 rather than allowing unauthenticated access.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zipline-ai-workflow-status-openapi.yml
  - https://zipline.ai/docs/running_on_zipline_hub/Auth
  type: http
slug: zipline-ai-authentication
source_filename: zipline-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://zipline.ai/docs/running_on_zipline_hub/Auth\ndocs: https://zipline.ai/docs/running_on_zipline_hub/Auth\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  overview: >-\n    Zipline supports optional authentication to secure access to the platform.\n    Users authenticate through the frontend (OAuth or SSO); backend services\n    (Orchestration, Eval) validate requests using signed JWTs verified\n    statelessly via JWKS. The CLI authenticates with the device authorization\n    flow (RFC 8628).\n  human_login: [OAuth 2.0, SSO (OIDC), SSO (SAML)]\n  service_auth: [Bearer JWT verified via JWKS]\n  cli_auth: [RFC 8628 device authorization flow]\nproviders:\n  - name: Google OAuth\n    type: oauth2\n    env: [GOOGLE_OAUTH_CLIENT_ID, GOOGLE_OAUTH_CLIENT_SECRET]\n    redirect_uri: \"{AUTH_URL}/api/auth/callback/google\"\n  - name: GitHub OAuth\n    type: oauth2\n    env: [GITHUB_OAUTH_CLIENT_ID, GITHUB_OAUTH_CLIENT_SECRET]\n\
  \  - name: SSO (OIDC / SAML)\n    type: openIdConnect\n    notes: Enterprise SSO via OIDC or SAML; SAML post-login redirect honors AUTH_EXTERNAL_URL behind a reverse proxy.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Short-lived JWT minted by `zipline auth get-access-token` (or issued to the\n      frontend after OAuth/SSO login). Backend services validate it statelessly\n      against the JWKS endpoint (AUTH_JWKS_URL, e.g. /api/auth/jwks). When\n      AUTH_ENABLED=true but the JWKS endpoint is unreachable, protected routes\n      return 503 rather than allowing unauthenticated access.\n    sources:\n      - openapi/zipline-ai-workflow-status-openapi.yml\n      - https://zipline.ai/docs/running_on_zipline_hub/Auth\nauthorization:\n  model: role-based (RBAC)\n  notes: Workflow Status API requires viewer access when role-based authorization is enabled.\n  allowlist: AUTH_ALLOWED_PRINCIPALS restricts sign-in to specific\
  \ domains or exact emails.\nconfig_env:\n  - AUTH_ENABLED\n  - AUTH_URL\n  - AUTH_EXTERNAL_URL\n  - AUTH_SECRET\n  - AUTH_ALLOWED_HOSTS\n  - AUTH_ALLOWED_PRINCIPALS\n  - AUTH_JWKS_URL\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zipline-ai/refs/heads/main/authentication/zipline-ai-authentication.yml
summary_line: http/oauth2/openIdConnect · 1 scheme
tags:
- Company
---
