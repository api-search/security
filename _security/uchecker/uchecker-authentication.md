---
api_key_in:
- header
api_specs:
- filename: uchecker-default-api-openapi.yml
  format: yaml
  label: uChecker Аутентификация API
  slug: uchecker-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uchecker/refs/heads/main/openapi/uchecker-default-api-openapi.yml
- filename: uchecker-email-api-openapi.yml
  format: yaml
  label: uChecker Валидация Email API
  slug: uchecker-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uchecker/refs/heads/main/openapi/uchecker-email-api-openapi.yml
- filename: uchecker-esp-api-openapi.yml
  format: yaml
  label: uChecker ESP Провайдеры API
  slug: uchecker-esp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uchecker/refs/heads/main/openapi/uchecker-esp-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Uchecker Authentication
name_suffix: Authentication
oauth_flows: []
overview: uChecker secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: uChecker
provider_slug: uchecker
scheme_count: 3
schemes:
- also_used_by:
  - 'The hosted MCP server at https://api.uchecker.net/mcp accepts the same key, either as an `x-api-key` header or as `Authorization: Bearer <key>`. Confirmed by live probe — an unauthenticated tools/list returned JSON-RPC error -32001 naming both header forms.'
  description: Персональный API ключ. Отображается в личном кабинете (https://app.uchecker.net). Передавайте в заголовке `x-api-key` каждого запроса. Ключ не имеет срока действия — действует до ручного сброса через `POST /auth/reset-api-key`.
  description_en: Personal API key, shown in the dashboard. Send it in the `x-api-key` header of every request. It does not expire; it is valid until manually reset.
  example_form: 'x-api-key: uk_xxxxxxxxxxxxx'
  expiry: none
  in: header
  key_prefix: uk_
  name: api-key
  obtain: https://app.uchecker.net (shown in the dashboard immediately after registration)
  parameter: x-api-key
  rotation: POST /auth/reset-api-key (AuthController_resetApiKey) — invalidates the old key immediately
  sources:
  - openapi/uchecker-default-api-openapi.yml
  - openapi/uchecker-email-api-openapi.yml
  - openapi/uchecker-esp-api-openapi.yml
  - https://uchecker.net/en/mcp
  type: apiKey
- access_token_ttl: 1 hour
  alternate_issue:
  - AuthController_telegramLogin (POST /auth/telegram-login) — same response shape, issued against a linked Telegram chat ID
  - AuthController_registerWithCode (POST /auth/register-with-code)
  bearerFormat: JWT
  description: JWT access token, полученный через `POST /auth/login`. Время жизни — 1 час. Для обновления используйте `POST /auth/refresh` с refresh token.
  description_en: JWT access token obtained via POST /auth/login. Lifetime 1 hour; renew with POST /auth/refresh using the refresh token.
  issue_operation: AuthController_login (POST /auth/login)
  name: bearer
  refresh_operation: AuthController_refresh (POST /auth/refresh)
  refresh_rotation: The 200 description on POST /auth/refresh states a NEW pair is returned and the old refresh token is retired — refresh tokens rotate.
  refresh_token_ttl: 7 days
  scheme: bearer
  sources:
  - openapi/uchecker-default-api-openapi.yml
  - openapi/uchecker-email-api-openapi.yml
  - openapi/uchecker-esp-api-openapi.yml
  type: http
- declared_in_spec: false
  description: NOT a declared securityScheme — inferred from the 401 descriptions on both ESP operations ("Токен ESP-провайдера отсутствует, невалиден или просрочен" / ESP provider token missing, invalid or expired). A partner-issued credential distinct from the ordinary `uk_` account key; there is no self-service path to obtain one.
  name: esp-provider-token
  obtain: partner arrangement — support@uchecker.net
  scope: /api/v1/esp/price, /api/v1/esp/provision
  sources:
  - openapi/uchecker-esp-api-openapi.yml
  type: bearer-token
slug: uchecker-authentication
source_filename: uchecker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: searched\nsource: >-\n  https://api.uchecker.net/docs/openapi.json — components.securitySchemes plus the\n  \"Аутентификация\" section of info.description; https://uchecker.net/en/mcp\ndocs: https://api.uchecker.net/docs\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  interchangeable: true\n  note: >-\n    Two equivalent schemes — either grants full access to every endpoint. uChecker\n    recommends the API key for server-side integrations (\"проще и не требует управления\n    токенами\") and the JWT for front-end applications. The ESP endpoints are the one\n    exception: they require a separate ESP provider token.\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  key_prefix: uk_\n  expiry: none\n  rotation: POST /auth/reset-api-key (AuthController_resetApiKey) — invalidates the old key immediately\n  obtain: https://app.uchecker.net\
  \ (shown in the dashboard immediately after registration)\n  example_form: 'x-api-key: uk_xxxxxxxxxxxxx'\n  description: >-\n    Персональный API ключ. Отображается в личном кабинете (https://app.uchecker.net).\n    Передавайте в заголовке `x-api-key` каждого запроса. Ключ не имеет срока действия —\n    действует до ручного сброса через `POST /auth/reset-api-key`.\n  description_en: >-\n    Personal API key, shown in the dashboard. Send it in the `x-api-key` header of every\n    request. It does not expire; it is valid until manually reset.\n  also_used_by:\n    - >-\n      The hosted MCP server at https://api.uchecker.net/mcp accepts the same key, either as\n      an `x-api-key` header or as `Authorization: Bearer <key>`. Confirmed by live probe —\n      an unauthenticated tools/list returned JSON-RPC error -32001 naming both header forms.\n  sources:\n  - openapi/uchecker-default-api-openapi.yml\n  - openapi/uchecker-email-api-openapi.yml\n  - openapi/uchecker-esp-api-openapi.yml\n \
  \ - https://uchecker.net/en/mcp\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  issue_operation: AuthController_login (POST /auth/login)\n  refresh_operation: AuthController_refresh (POST /auth/refresh)\n  access_token_ttl: 1 hour\n  refresh_token_ttl: 7 days\n  refresh_rotation: >-\n    The 200 description on POST /auth/refresh states a NEW pair is returned and the old\n    refresh token is retired — refresh tokens rotate.\n  alternate_issue:\n    - AuthController_telegramLogin (POST /auth/telegram-login) — same response shape, issued against a linked Telegram chat ID\n    - AuthController_registerWithCode (POST /auth/register-with-code)\n  description: >-\n    JWT access token, полученный через `POST /auth/login`. Время жизни — 1 час. Для\n    обновления используйте `POST /auth/refresh` с refresh token.\n  description_en: >-\n    JWT access token obtained via POST /auth/login. Lifetime 1 hour; renew with\n    POST /auth/refresh using the refresh token.\n  sources:\n\
  \  - openapi/uchecker-default-api-openapi.yml\n  - openapi/uchecker-email-api-openapi.yml\n  - openapi/uchecker-esp-api-openapi.yml\n- name: esp-provider-token\n  type: bearer-token\n  declared_in_spec: false\n  scope: /api/v1/esp/price, /api/v1/esp/provision\n  description: >-\n    NOT a declared securityScheme — inferred from the 401 descriptions on both ESP\n    operations (\"Токен ESP-провайдера отсутствует, невалиден или просрочен\" / ESP provider\n    token missing, invalid or expired). A partner-issued credential distinct from the\n    ordinary `uk_` account key; there is no self-service path to obtain one.\n  obtain: partner arrangement — support@uchecker.net\n  sources:\n  - openapi/uchecker-esp-api-openapi.yml\noauth:\n  supported: false\n  probes:\n    - url: https://api.uchecker.net/.well-known/oauth-authorization-server\n      status: 404\n    - url: https://api.uchecker.net/.well-known/oauth-protected-resource\n      status: 404\n    - url: https://api.uchecker.net/.well-known/openid-configuration\n\
  \      status: 404\n  note: >-\n    No OAuth 2.0 or OpenID Connect anywhere, including on the MCP endpoint — the MCP server\n    authenticates with the same static API key rather than an OAuth flow. See\n    scopes/ (absent: no oauth2 securityScheme, so there is nothing to derive).\nfailure_modes:\n  - status: 401\n    meaning: Missing or invalid API key / JWT, or an expired access token.\n  - status: 403\n    meaning: >-\n      Authenticated but not permitted — insufficient credits, or a feature (the affiliate\n      programme) not enabled on the account. Authentication succeeded; authorisation or\n      quota failed.\ntransport_security:\n  https_only: true\n  tls: TLSv1.3\n  hsts: max-age=31536000\n  see_also: security/uchecker-domain-security.yml\ngaps_for_the_provider:\n  - Declare the ESP provider token as a securityScheme instead of leaving it in prose.\n  - Document the API key entropy/format beyond the `uk_` prefix.\n  - No scoped keys: one key grants full access to validation,\
  \ billing and account management.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uchecker/refs/heads/main/authentication/uchecker-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Email Verification
- Email
- SMTP
- DNS
- Deliverability
- mx
- SPF
- DKIM
- DMARC
- MCP
- agent-native
- Data Quality
---
