---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Mirelo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mirelo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mirelo
provider_slug: mirelo
scheme_count: 1
schemes:
- description: 'All requests to the Mirelo API (https://api.mirelo.ai/v2/) are authenticated with a secret API key passed as a bearer token in the Authorization header: `Authorization: Bearer sk-...`. API keys are issued from the Mirelo Studio account dashboard. Keys carry the account''s credit balance; there is no OAuth or per-scope authorization surface.'
  header: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - https://mirelo.ai/api-docs
  token_prefix: sk-
  type: http
slug: mirelo-authentication
source_filename: mirelo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://mirelo.ai/api-docs\ndocs: https://mirelo.ai/api-docs\nsummary:\n  types:\n  - http\n  scheme: bearer\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    All requests to the Mirelo API (https://api.mirelo.ai/v2/) are authenticated\n    with a secret API key passed as a bearer token in the Authorization header:\n    `Authorization: Bearer sk-...`. API keys are issued from the Mirelo Studio\n    account dashboard. Keys carry the account's credit balance; there is no\n    OAuth or per-scope authorization surface.\n  token_prefix: sk-\n  header: Authorization\n  sources:\n  - https://mirelo.ai/api-docs\nnotes: >-\n  Key-auth provider (single secret bearer token). No OAuth2/OIDC and no scope\n  surface, so scopes/ is intentionally not produced.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirelo/refs/heads/main/authentication/mirelo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai Ml
- Audio
- Sound Effects
- Generative AI
- Video
- Text to Audio
- Audio to MIDI
- Machine Learning
---
