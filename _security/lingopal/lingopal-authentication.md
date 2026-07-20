---
api_key_in:
- header
api_specs:
- filename: lingopal-openapi-original.json
  format: json
  label: Lingopal API v2
  slug: lingopal-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lingopal/refs/heads/main/openapi/lingopal-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Lingopal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lingopal secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lingopal
provider_slug: lingopal
scheme_count: 1
schemes:
- applied: global
  docs: https://docs.lingopal.ai/guides/authentication
  in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/lingopal-openapi-original.json
  type: apiKey
slug: lingopal-authentication
source_filename: lingopal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/lingopal-openapi-original.json\ndocs: https://docs.lingopal.ai/guides/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  bearer_tokens: false\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  applied: global\n  sources:\n  - openapi/lingopal-openapi-original.json\n  docs: https://docs.lingopal.ai/guides/authentication\nkey_management:\n  issue: Lingopal dashboard (https://app.lingopal.ai/login) or account contact\n  rotate: Lingopal dashboard or account contact\n  revoke: Lingopal dashboard or account contact\n  environment_separation: >-\n    The docs recommend separate keys for development and production \"when available\";\n    no test-vs-live key prefix or sandbox mode is published.\nguidance:\n- Store the key server-side in an environment variable (documented as LINGOPAL_API_KEY).\n- Never commit a key or place it in browser-side\
  \ code.\n- Keep .env files out of version control.\n- Rotate a key immediately if it is exposed.\n- Do not attach X-API-Key to presigned storage upload URLs returned by createStorageUpload.\nfailure_mode:\n  status: 401\n  meaning: >-\n    Header missing or key invalid. Confirm the header name is exactly X-API-Key, that\n    the environment variable is populated, and that the key has not been revoked.\nnotes: >-\n  There is no OAuth, OIDC, mTLS, or scope surface on this API, so no scopes/ artifact\n  is emitted. Key auth with no scopes is the whole authorization model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lingopal/refs/heads/main/authentication/lingopal-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Frontier Tech
- Artificial Intelligence
- Translation
- Localization
- Speech
- Media
- Broadcasting
- Video
- Subtitles
- Voice Cloning
---
