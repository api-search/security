---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
- http
description: AltScore authenticates through a Frontegg-backed OAuth 2.0 / OpenID Connect identity service at auth.altscore.ai. The SDK and CLI accept several credential types; the primary machine-to-machine path is client_id + client_secret exchanged for an access token (with refresh) at the identity token endpoint. Requests are multi-tenant — a tenant is resolved from the token. A dedicated sandbox identity host (auth.sandbox.altscore.ai) mirrors production.
kind: authentication
layout: security
method: searched
name: Altscore Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- refreshToken
- deviceCode
- tokenExchange
overview: AltScore secures its APIs with oauth2, apiKey, and http across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, refreshToken, deviceCode, and tokenExchange flow(s).
provider_name: AltScore
provider_slug: altscore
scheme_count: 5
schemes:
- description: Machine-to-machine. POST client_id + client_secret to /identity/resources/auth/v1/api-token; returns accessToken + refreshToken. Env vars ALTSCORE_CLIENT_ID / ALTSCORE_CLIENT_SECRET. This is the default SDK and CLI credential.
  flow: clientCredentials
  name: client_credentials
  refresh_endpoint: https://auth.altscore.ai/identity/resources/auth/v2/api-token/token/refresh
  sources:
  - https://github.com/AltScore/altscore-python
  token_endpoint: https://auth.altscore.ai/identity/resources/auth/v1/api-token
  type: oauth2
- description: Email + password login at /identity/resources/auth/v1/user; returns an accessToken (user token). Env vars ALTSCORE_EMAIL / ALTSCORE_PASSWORD.
  flow: password
  name: user_credentials
  sources:
  - https://github.com/AltScore/altscore-python
  token_endpoint: https://auth.altscore.ai/identity/resources/auth/v1/user
  type: oauth2
- description: Static API key accepted by the SDK/CLI (api_key parameter). Used in place of an interactive login for programmatic access.
  in: header
  name: api_key
  sources:
  - https://github.com/AltScore/altscore-python
  type: apiKey
- bearerFormat: JWT
  description: Bearer access token (JWT) issued by the identity service; carries the tenant claim. Auto-refreshed by the SDK/CLI on 401.
  name: user_token
  scheme: bearer
  sources:
  - https://github.com/AltScore/altscore-python
  type: http
- description: Scoped token used for borrower self-service sign-up flows (borrower_sign_up_with_form).
  in: header
  name: form_token
  sources:
  - https://github.com/AltScore/altscore-python
  type: apiKey
slug: altscore-authentication
source_filename: altscore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: >-\n  https://github.com/AltScore/altscore-python (src/altscore/__init__.py) and the\n  live OIDC discovery document at\n  https://auth.altscore.ai/.well-known/openid-configuration\ndescription: >-\n  AltScore authenticates through a Frontegg-backed OAuth 2.0 / OpenID Connect\n  identity service at auth.altscore.ai. The SDK and CLI accept several credential\n  types; the primary machine-to-machine path is client_id + client_secret\n  exchanged for an access token (with refresh) at the identity token endpoint.\n  Requests are multi-tenant — a tenant is resolved from the token. A dedicated\n  sandbox identity host (auth.sandbox.altscore.ai) mirrors production.\nsummary:\n  types: [oauth2, apiKey, http]\n  oauth2_flows: [clientCredentials, authorizationCode, refreshToken, deviceCode, tokenExchange]\n  api_key_in: [header]\nidentity_service:\n  provider: Frontegg\n  issuer: https://auth.altscore.ai\n  authorization_endpoint: https://auth.altscore.ai/oauth/authorize\n\
  \  token_endpoint: https://auth.altscore.ai/oauth/token\n  jwks: see well-known/altscore-openid-configuration.json\n  sandbox_issuer: https://auth.sandbox.altscore.ai\nschemes:\n- name: client_credentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Machine-to-machine. POST client_id + client_secret to\n    /identity/resources/auth/v1/api-token; returns accessToken + refreshToken.\n    Env vars ALTSCORE_CLIENT_ID / ALTSCORE_CLIENT_SECRET. This is the default SDK\n    and CLI credential.\n  token_endpoint: https://auth.altscore.ai/identity/resources/auth/v1/api-token\n  refresh_endpoint: https://auth.altscore.ai/identity/resources/auth/v2/api-token/token/refresh\n  sources: [https://github.com/AltScore/altscore-python]\n- name: user_credentials\n  type: oauth2\n  flow: password\n  description: >-\n    Email + password login at /identity/resources/auth/v1/user; returns an\n    accessToken (user token). Env vars ALTSCORE_EMAIL / ALTSCORE_PASSWORD.\n  token_endpoint:\
  \ https://auth.altscore.ai/identity/resources/auth/v1/user\n  sources: [https://github.com/AltScore/altscore-python]\n- name: api_key\n  type: apiKey\n  in: header\n  description: >-\n    Static API key accepted by the SDK/CLI (api_key parameter). Used in place of\n    an interactive login for programmatic access.\n  sources: [https://github.com/AltScore/altscore-python]\n- name: user_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Bearer access token (JWT) issued by the identity service; carries the tenant\n    claim. Auto-refreshed by the SDK/CLI on 401.\n  sources: [https://github.com/AltScore/altscore-python]\n- name: form_token\n  type: apiKey\n  in: header\n  description: >-\n    Scoped token used for borrower self-service sign-up flows\n    (borrower_sign_up_with_form).\n  sources: [https://github.com/AltScore/altscore-python]\nnotes: >-\n  Tokens auto-refresh on 401 (no manual refresh needed). The CLI can export the\n  active credentials as env\
  \ vars for the Python SDK via `altscore env`.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altscore/refs/heads/main/authentication/altscore-authentication.yml
summary_line: oauth2/apiKey/http · 5 schemes
tags:
- Company
- Credit
- Lending
- Fintech
- Credit Scoring
- Underwriting
- KYC
- Financial Services
- Latin America
- Data Aggregation
- Workflows
- Decisioning
---
