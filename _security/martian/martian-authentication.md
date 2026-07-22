---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Martian Authentication
name_suffix: Authentication
oauth_flows: []
overview: Martian secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Martian
provider_slug: martian
scheme_count: 1
schemes:
- description: The Martian Gateway API uses API keys with bearer token authentication. Include the API key in the Authorization header of every request. Keys are created and managed in the Martian Dashboard (app.withmartian.com) under the API Keys section.
  format: 'Authorization: Bearer <API_KEY>'
  header_name: Authorization
  in: header
  name: BearerApiKey
  scheme: bearer
  sources:
  - docs.withmartian.com/api-reference/authentication
  type: http
slug: martian-authentication
source_filename: martian-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.withmartian.com/api-reference/authentication\ndocs: https://docs.withmartian.com/api-reference/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  header: Authorization\n  scheme: bearer\n  oauth2_flows: []\nschemes:\n- name: BearerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  header_name: Authorization\n  format: 'Authorization: Bearer <API_KEY>'\n  description: >-\n    The Martian Gateway API uses API keys with bearer token authentication.\n    Include the API key in the Authorization header of every request. Keys are\n    created and managed in the Martian Dashboard (app.withmartian.com) under the\n    API Keys section.\n  sources: [docs.withmartian.com/api-reference/authentication]\nkey_management:\n  dashboard: https://app.withmartian.com/\n  create: Sign up or log in, navigate to API Keys, create or copy a key.\n  rotation: Rotate keys periodically and immediately if compromised;\
  \ revoke and\n    regenerate in the Dashboard.\nguidance:\n- Never commit API keys to version control or expose them in client-side code.\n- Store keys in environment variables or a secrets manager (MARTIAN_API_KEY).\n- Monitor usage in the Martian Dashboard to detect unauthorized access.\nnotes: >-\n  No OAuth 2.0 / OpenID Connect surface is documented; authentication is\n  API-key-only. When using the official OpenAI or Anthropic SDKs the key is\n  supplied as the SDK api_key with base_url set to https://api.withmartian.com/v1.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/martian/refs/heads/main/authentication/martian-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- LLM
- LLM Gateway
- Model Router
- Machine Learning
- Interpretability
- Inference
- OpenAI Compatible
- Developer Tools
---
