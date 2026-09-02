---
api_key_in:
- header
api_specs:
- filename: ahasend-accounts-api-openapi.yml
  format: yaml
  label: AhaSend Accounts API
  slug: ahasend-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-accounts-api-openapi.yml
- filename: ahasend-api-keys-api-openapi.yml
  format: yaml
  label: AhaSend API Keys API
  slug: ahasend-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-api-keys-api-openapi.yml
- filename: ahasend-domains-api-openapi.yml
  format: yaml
  label: AhaSend Domains API
  slug: ahasend-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-domains-api-openapi.yml
- filename: ahasend-email-api-openapi.yml
  format: yaml
  label: AhaSend Email API
  slug: ahasend-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-email-api-openapi.yml
- filename: ahasend-messages-api-openapi.yml
  format: yaml
  label: AhaSend Messages API
  slug: ahasend-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-messages-api-openapi.yml
- filename: ahasend-routes-api-openapi.yml
  format: yaml
  label: AhaSend Routes API
  slug: ahasend-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-routes-api-openapi.yml
- filename: ahasend-smtp-credentials-api-openapi.yml
  format: yaml
  label: AhaSend SMTP Credentials API
  slug: ahasend-smtp-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-smtp-credentials-api-openapi.yml
- filename: ahasend-statistics-api-openapi.yml
  format: yaml
  label: AhaSend Statistics API
  slug: ahasend-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-statistics-api-openapi.yml
- filename: ahasend-suppressions-api-openapi.yml
  format: yaml
  label: AhaSend Suppressions API
  slug: ahasend-suppressions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-suppressions-api-openapi.yml
- filename: ahasend-utility-api-openapi.yml
  format: yaml
  label: AhaSend Utility API
  slug: ahasend-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-utility-api-openapi.yml
- filename: ahasend-webhooks-api-openapi.yml
  format: yaml
  label: AhaSend Webhooks API
  slug: ahasend-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-webhooks-api-openapi.yml
- filename: ahasend-sub-accounts-api-openapi.yml
  format: yaml
  label: AhaSend Sub Accounts API
  slug: ahasend-sub-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-sub-accounts-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ahasend Authentication
name_suffix: Authentication
oauth_flows: []
overview: AhaSend secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AhaSend
provider_slug: ahasend
scheme_count: 1
schemes:
- bearerFormat: aha-sk- followed by a 64-character random string
  description: 'The single authentication scheme for the whole API v2 surface, applied globally and refined per operation. The contract''s own note explains the refinement: "Non-empty Security Requirement values are AhaSend API-key roles. Roles listed within one requirement object are jointly required; separate requirement objects are alternatives." So the security block does double duty as the authorization model — see scopes/ahasend-scopes.yml.'
  header: 'Authorization: Bearer <api_key>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/_original/ahasend-openapi-v2.yaml
  - https://ahasend.com/docs/api-reference/authentication.md
  type: http
slug: ahasend-authentication
source_filename: ahasend-authentication.yml
source_heading: Authentication Profile
source_url: https://ahasend.com/docs/api-reference/authentication.md
source_yaml: "generated: '2026-08-30'\nmethod: searched\ndocs: https://ahasend.com/docs/api-reference/authentication\nsource: https://ahasend.com/docs/api-reference/authentication\nsources:\n  - https://ahasend.com/docs/api-reference/authentication.md\n  - https://ahasend.com/docs/send-api/credentials.md\n  - https://ahasend.com/docs/security/scoped-credentials.md\n  - https://ahasend.com/docs/security/ip-allow-lists.md\n  - https://ahasend.com/docs/security/sso.md\n  - openapi/_original/ahasend-openapi-v2.yaml\nprovider: AhaSend\nproviderId: ahasend\nsummary:\n  types:\n    - http\n  api_key_in:\n    - header\n  oauth2: false\n  openIdConnect: false\n  mutualTLS: false\nschemes:\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: aha-sk- followed by a 64-character random string\n    header: 'Authorization: Bearer <api_key>'\n    description: >-\n      The single authentication scheme for the whole API v2 surface, applied globally and refined\n      per operation.\
  \ The contract's own note explains the refinement: \"Non-empty Security\n      Requirement values are AhaSend API-key roles. Roles listed within one requirement object are\n      jointly required; separate requirement objects are alternatives.\" So the security block does\n      double duty as the authorization model — see scopes/ahasend-scopes.yml.\n    sources:\n      - openapi/_original/ahasend-openapi-v2.yaml\n      - https://ahasend.com/docs/api-reference/authentication.md\nkey_management:\n  create: createAPIKey (POST /v2/accounts/{account_id}/api-keys)\n  secret_visibility: >-\n    The `secret_key` is returned once, on the 201. Every list/get/update/delete response omits it.\n    An exact idempotent retry replays it for 5 minutes only; after that the key must be recreated.\n  public_identifier: APIKey.public_key\n  last_used: APIKey.last_used_at is exposed, so an unused key is detectable.\n  rotation: >-\n    No automatic key rotation and no expiry field. Rotation means create-then-delete\
  \ by hand.\n    (DKIM keys, by contrast, rotate automatically on a configurable interval.)\nrestrictions:\n  scoped_keys:\n    supported: true\n    description: >-\n      Every key carries an explicit scope list, including per-domain scopes such as\n      messages:send:{example.com}. See scopes/ahasend-scopes.yml for all 51.\n  ip_allow_list:\n    supported: true\n    field: APIKey.ip_allow_list\n    limits: up to 100 IPv4/IPv6 addresses or CIDR ranges per key\n    semantics: >-\n      A key with a non-empty allow list is rejected on EVERY endpoint from any other IP,\n      regardless of scopes. An empty list means no restriction. \"Allow everything\" ranges are\n      rejected.\n    self_lockout_protection: >-\n      Setting a key's own allow list to a value excluding the calling IP is rejected and nothing is\n      saved. The dashboard is never blocked by a key's allow list.\n    change_control: >-\n      Changing an allow list in the dashboard re-prompts for a 2FA code (or password),\
  \ remembered\n      for 5 minutes, and emails owners and administrators that a security setting changed.\n  sandbox_mode:\n    description: >-\n      A credential can be created in, or switched to, Sandbox mode — sends made with it are always\n      simulated. Sandbox and production keys share the aha-sk- prefix, so the mode is NOT visible\n      in the key string.\nsmtp_authentication:\n  mechanism: PLAIN over STARTTLS\n  hosts: [send.ahasend.com, send-us.ahasend.com]\n  ports: [25, 587, 2525]\n  note: >-\n    Implicit TLS (SMTPS) on port 465 is explicitly not supported. SMTP credentials are separate\n    objects from API keys, created in the dashboard or through the SMTP Credentials API, and can\n    themselves be global or domain-scoped.\nwebhook_authentication:\n  direction: inbound-to-subscriber\n  mechanism: Standard Webhooks HMAC-SHA256 over `id.timestamp.body`\n  see: asyncapi/ahasend-webhooks.yml\nhuman_authentication:\n  two_factor: TOTP-based 2FA, with account-wide enforcement\
  \ available\n  sso:\n    protocol: OpenID Connect\n    role: relying-party\n    features: [PKCE, multi-domain]\n    plan: Max\n    note: Dashboard login only. AhaSend does not issue OAuth or OIDC tokens for its API.\ngaps:\n  - No OAuth 2.0 or OIDC authorization for API access — API keys only.\n  - No key expiry, no automatic rotation, no published key-rotation guidance.\n  - No /.well-known/oauth-authorization-server or /.well-known/openid-configuration (both 404).\n  - >-\n    A 403 caused by a missing scope and a 403 caused by an IP-allow-list rejection are not\n    distinguishable from the response body.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/authentication/ahasend-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhook
---
