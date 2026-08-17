---
api_key_in:
- header
api_specs:
- filename: lalal-ai-batch-stem-separation-api-openapi.yml
  format: yaml
  label: LALAL.AI Batch Stem Separation API
  slug: lalal-ai-batch-stem-separation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lalal-ai/refs/heads/main/openapi/lalal-ai-batch-stem-separation-api-openapi.yml
- filename: lalal-ai-common-api-openapi.yml
  format: yaml
  label: LALAL.AI Common API
  slug: lalal-ai-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lalal-ai/refs/heads/main/openapi/lalal-ai-common-api-openapi.yml
- filename: lalal-ai-stem-separation-api-openapi.yml
  format: yaml
  label: LALAL.AI Stem Separation API
  slug: lalal-ai-stem-separation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lalal-ai/refs/heads/main/openapi/lalal-ai-stem-separation-api-openapi.yml
- filename: lalal-ai-voice-change-api-openapi.yml
  format: yaml
  label: LALAL.AI Voice Change API
  slug: lalal-ai-voice-change-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lalal-ai/refs/heads/main/openapi/lalal-ai-voice-change-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Lalal Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: LALAL.AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LALAL.AI
provider_slug: lalal-ai
scheme_count: 1
schemes:
- applied_to: 'all 15 v1 operations (security [{ApiKeyHeaderAuth: []}] on every operation)'
  in: header
  name: ApiKeyHeaderAuth
  parameter: X-License-Key
  sources:
  - openapi/lalal-ai-common-api-openapi.yml
  - openapi/lalal-ai-stem-separation-api-openapi.yml
  - openapi/lalal-ai-batch-stem-separation-api-openapi.yml
  - openapi/lalal-ai-voice-change-api-openapi.yml
  - openapi/_original/lalal-ai-api-openapi.yml
  type: apiKey
slug: lalal-ai-authentication
source_filename: lalal-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/lalal-ai-api-openapi.yml\ndocs: https://www.lalal.ai/api/v1/docs/\nprovider: LALAL.AI\nprovider_id: lalal-ai\n\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  scopes: 0\n\nschemes:\n- name: ApiKeyHeaderAuth\n  type: apiKey\n  in: header\n  parameter: X-License-Key\n  applied_to: 'all 15 v1 operations (security [{ApiKeyHeaderAuth: []}] on every operation)'\n  sources:\n  - openapi/lalal-ai-common-api-openapi.yml\n  - openapi/lalal-ai-stem-separation-api-openapi.yml\n  - openapi/lalal-ai-batch-stem-separation-api-openapi.yml\n  - openapi/lalal-ai-voice-change-api-openapi.yml\n  - openapi/_original/lalal-ai-api-openapi.yml\n\ncredential:\n  kind: account license key\n  name: license key\n  obtained_from: https://www.lalal.ai/pricing/\n  entitlement: >-\n    API access requires a Pro plan or a minute top-up pack. Per the provider's llms.txt — \"API access is\n    available with\
  \ the Pro plan or any minute top-up pack - no subscription required\". The free Starter\n    plan does not grant API access.\n  scoped: false\n  rotatable_via_api: false\n  expiring: false\n  prefix: none\n  test_counterpart: none\n  note: >-\n    One long-lived, unscoped credential per account, carrying the full surface — including the destructive\n    cancel_cancel_all and delete_delete operations and the billable split operations. There is no\n    read-only key, no per-integration key and no programmatic rotation. Treat it as a root credential:\n    server-side only, one per integration boundary you can afford to revoke by hand.\n\nobserved_behavior:\n  probed: '2026-08-13'\n  url: https://www.lalal.ai/api/v1/check/\n  missing_credential_status: 403\n  missing_credential_body: '{\"detail\": \"Provide license key in ''X-License-Key'' header\"}'\n  www_authenticate: absent\n  note: >-\n    A missing credential answers 403, not 401, and returns no WWW-Authenticate challenge. Client code\
  \ that\n    branches on 401 to trigger a re-auth path will never fire.\n  cors:\n    access_control_allow_origin: '*'\n    access_control_allow_headers: Authorization,Content-Disposition,Content-Type,Cache-Control,Keep-Alive,Origin\n    warning: >-\n      Wildcard CORS permits the license key to be sent from a browser. Do not ship it to a client — it is\n      an account credential with billing and delete authority.\n\noauth2:\n  supported: false\n  evidence:\n    - no oauth2 securityScheme in the OpenAPI document\n    - https://www.lalal.ai/.well-known/oauth-authorization-server returned HTTP 404 on 2026-08-13\n    - https://www.lalal.ai/.well-known/openid-configuration returned HTTP 404 on 2026-08-13\n  note: >-\n    No OAuth and no OIDC, so there is no scopes/ artifact for this provider — nothing to enumerate.\n\nsuperseded_scheme:\n  version: v0\n  header: 'Authorization: license <key>'\n  status: deprecated\n  docs: https://www.lalal.ai/api/help/\n  note: >-\n    API v0 used a different\
  \ header entirely. Migrating from v0 to v1 is an authentication change, not just\n    a path change.\n\ncross_references:\n  - conventions/lalal-ai-conventions.yml\n  - errors/lalal-ai-problem-types.yml\n  - sandbox/lalal-ai-sandbox.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lalal-ai/refs/heads/main/authentication/lalal-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Artificial Intelligence
- Audio
- Audio Processing
- Stem Separation
- Vocal Removal
- Voice Cleaning
- Voice Cloning
- Voice Changer
- Music
- Machine Learning
- DSP
---
