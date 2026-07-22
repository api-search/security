---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Witai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wit.AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wit.AI
provider_slug: witai
scheme_count: 1
schemes:
- bearerFormat: opaque-token
  description: 'Every Wit HTTP API request is authenticated with a Server Access Token passed as an HTTP Bearer credential in the Authorization header (`Authorization: Bearer $TOKEN`). Each Wit app has its own token, found in the app''s Settings page (wit.ai/apps → Settings). A separate Client Access Token exists for lighter client-side use. Tokens are opaque and long-lived; there is no OAuth 2.0 authorization flow and no scope surface — access is scoped to the single Wit app the token belongs to.'
  location: header
  name: serverAccessToken
  parameter: Authorization
  scheme: bearer
  sources:
  - https://wit.ai/docs/http/latest
  type: http
slug: witai-authentication
source_filename: witai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://wit.ai/docs/http/latest + wit-ai SDK READMEs (node-wit, wit-go,\n  pywit). Wit.ai publishes no OpenAPI, so this profile is captured from the\n  documented HTTP auth model rather than derived from a spec.\ndocs: https://wit.ai/docs/http/latest\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: serverAccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: opaque-token\n  description: >-\n    Every Wit HTTP API request is authenticated with a Server Access Token\n    passed as an HTTP Bearer credential in the Authorization header\n    (`Authorization: Bearer $TOKEN`). Each Wit app has its own token, found in\n    the app's Settings page (wit.ai/apps → Settings). A separate Client Access\n    Token exists for lighter client-side use. Tokens are opaque and long-lived;\n    there is no OAuth 2.0 authorization flow and no scope surface — access is\n    scoped to the single Wit\
  \ app the token belongs to.\n  location: header\n  parameter: Authorization\n  sources:\n  - https://wit.ai/docs/http/latest\nnotes: >-\n  No OAuth2 / OpenID Connect / mTLS / API-key-in-query schemes are documented;\n  scopes/ is therefore not applicable. Token management (rotate/revoke) is done\n  in the Wit app dashboard.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/witai/refs/heads/main/authentication/witai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Natural Language Processing
- NLP
- Speech Recognition
- Speech to Text
- Text to Speech
- Intents
- Entities
- Voice
- Conversational AI
- Machine Learning
- Meta
---
