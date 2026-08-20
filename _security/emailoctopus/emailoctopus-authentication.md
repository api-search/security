---
api_key_in: []
api_specs:
- filename: emailoctopus-automation-api-openapi.yml
  format: yaml
  label: EmailOctopus Automation API
  slug: emailoctopus-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-automation-api-openapi.yml
- filename: emailoctopus-campaign-api-openapi.yml
  format: yaml
  label: EmailOctopus Campaign API
  slug: emailoctopus-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-campaign-api-openapi.yml
- filename: emailoctopus-contact-api-openapi.yml
  format: yaml
  label: EmailOctopus Contact API
  slug: emailoctopus-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-contact-api-openapi.yml
- filename: emailoctopus-field-api-openapi.yml
  format: yaml
  label: EmailOctopus Field API
  slug: emailoctopus-field-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-field-api-openapi.yml
- filename: emailoctopus-list-api-openapi.yml
  format: yaml
  label: EmailOctopus List API
  slug: emailoctopus-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-list-api-openapi.yml
- filename: emailoctopus-tag-api-openapi.yml
  format: yaml
  label: EmailOctopus Tag API
  slug: emailoctopus-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-tag-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Emailoctopus Authentication
name_suffix: Authentication
oauth_flows: []
overview: EmailOctopus secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EmailOctopus
provider_slug: emailoctopus
scheme_count: 1
schemes:
- description: 'Bearer API key in the Authorization header. Verbatim from the spec: "You can obtain your API key at https://api.emailoctopus.com/developer/api-keys/create".'
  format: Bearer {token}
  header: Authorization
  in: header
  key_creation_url: https://api.emailoctopus.com/developer/api-keys/create
  key_management_docs: https://help.emailoctopus.com/article/94-api-documentation
  name: api_key
  scheme: bearer
  sources:
  - openapi/_original/emailoctopus-v2-openapi.json
  - openapi/emailoctopus-list-api-openapi.yml
  - openapi/emailoctopus-contact-api-openapi.yml
  - openapi/emailoctopus-campaign-api-openapi.yml
  - openapi/emailoctopus-tag-api-openapi.yml
  - openapi/emailoctopus-field-api-openapi.yml
  - openapi/emailoctopus-automation-api-openapi.yml
  type: http
slug: emailoctopus-authentication
source_filename: emailoctopus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/emailoctopus-v2-openapi.json\ndocs: https://emailoctopus.com/api-documentation/v2\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  schemes_count: 1\n  global_security: true\nmodel: >-\n  A single account-wide API key presented as an HTTP Bearer token. There is no OAuth, no\n  OIDC, no scope model, no key rotation API and no per-key permission surface — one key\n  grants full access to everything in the account it belongs to. The scheme is applied\n  globally in the spec (top-level `security: [{api_key: []}]`), so every one of the 25\n  operations requires it; none are public.\nschemes:\n- name: api_key\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer {token}'\n  description: >-\n    Bearer API key in the Authorization header. Verbatim from the spec: \"You can obtain\n    your API key at https://api.emailoctopus.com/developer/api-keys/create\".\n\
  \  key_creation_url: https://api.emailoctopus.com/developer/api-keys/create\n  key_management_docs: https://help.emailoctopus.com/article/94-api-documentation\n  sources:\n  - openapi/_original/emailoctopus-v2-openapi.json\n  - openapi/emailoctopus-list-api-openapi.yml\n  - openapi/emailoctopus-contact-api-openapi.yml\n  - openapi/emailoctopus-campaign-api-openapi.yml\n  - openapi/emailoctopus-tag-api-openapi.yml\n  - openapi/emailoctopus-field-api-openapi.yml\n  - openapi/emailoctopus-automation-api-openapi.yml\nkey_versioning:\n  legacy_cutover: '2024-10-07'\n  note: >-\n    API keys minted before the v2 launch on 2024-10-07 are labelled \"legacy\" in the\n    dashboard and DO NOT authenticate against v2 — the API answers `401` with\n    `\"Invalid key.\"` and type `#unauthorized`. Keys created after that date are described\n    by EmailOctopus as \"compatible with all versions of the API\". This makes the API key\n    the de facto version selector, since the URL carries no version segment.\n\
  scopes:\n  supported: false\n  note: >-\n    No scope or permission model exists, so scopes/ is intentionally absent from this repo\n    rather than written as an empty artifact.\nfailure_modes:\n  - status: 401\n    type: https://emailoctopus.com/api-documentation/v2#unauthorized\n    meaning: Key missing, malformed, or legacy (pre-2024-10-07).\n    probed: true\n  - status: 403\n    type: https://emailoctopus.com/api-documentation/v2#access-denied\n    meaning: >-\n      Valid key, wrong account. EmailOctopus's documented check is to compare the last four\n      characters of the key against the keys listed on the target account.\nwebhook_authentication:\n  direction: inbound\n  mechanism: HMAC-SHA256 over the raw request body, hex, prefixed \"sha256=\"\n  header: EmailOctopus-Signature\n  note: Separate from API-key auth; see asyncapi/emailoctopus-webhooks.yml.\nx-evidence:\n  - url: https://emailoctopus.com/api-documentation/v2\n    http_status: 200\n    kind: openapi-and-reference\n\
  \  - url: https://api.emailoctopus.com/lists\n    http_status: 401\n    kind: live-probe-no-credential\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/authentication/emailoctopus-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- Email Marketing
- Newsletters
- Campaigns
- Automation
- Contacts
- List
- Marketing
- Webhook
- Transactional Email
- Subscriber Management
- Reporting
---
