---
api_key_in:
- header
auth_types:
- apiKey
description: Authentication profile for the Unsloth local API (2026-07-21). Unsloth has no hosted API; models loaded in Unsloth Studio are exposed on the user's own machine as an authenticated OpenAI/Anthropic-compatible endpoint via llama-server. Keys are created in Studio (Settings -> API) or auto-created by `unsloth run`; Unsloth stores only a hash and shows the key once. Requests with a revoked key fail 401 Unauthorized. No OpenAPI is published, so this profile is captured from the docs rather than derived from a spec.
kind: authentication
layout: security
method: searched
name: Unsloth Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unsloth secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unsloth
provider_slug: unsloth
scheme_count: 1
schemes:
- expiry: Optional expiry settable at key creation.
  header: Authorization (Bearer)
  in: header
  key_prefix: sk-unsloth-
  name: UnslothApiKey
  revocation: Keys revocable in Studio Settings -> API; revoked keys return 401 Unauthorized.
  scope: local instance only (http://localhost:PORT base URL)
  sources:
  - https://unsloth.ai/docs/basics/api
  type: apiKey
slug: unsloth-authentication
source_filename: unsloth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://unsloth.ai/docs/basics/api\nsource: https://unsloth.ai/docs/basics/api\ndescription: >-\n  Authentication profile for the Unsloth local API (2026-07-21). Unsloth has\n  no hosted API; models loaded in Unsloth Studio are exposed on the user's own\n  machine as an authenticated OpenAI/Anthropic-compatible endpoint via\n  llama-server. Keys are created in Studio (Settings -> API) or auto-created\n  by `unsloth run`; Unsloth stores only a hash and shows the key once.\n  Requests with a revoked key fail 401 Unauthorized. No OpenAPI is published,\n  so this profile is captured from the docs rather than derived from a spec.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: UnslothApiKey\n    type: apiKey\n    in: header\n    header: Authorization (Bearer)\n    key_prefix: sk-unsloth-\n    scope: local instance only (http://localhost:PORT base URL)\n    revocation: Keys revocable in\
  \ Studio Settings -> API; revoked keys return 401 Unauthorized.\n    expiry: Optional expiry settable at key creation.\n    sources: [https://unsloth.ai/docs/basics/api]\nendpoints:\n  - path: /v1/chat/completions\n    dialect: OpenAI-compatible\n  - path: /v1/responses\n    dialect: OpenAI-compatible\n  - path: /v1/messages\n    dialect: Anthropic-compatible\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unsloth/refs/heads/main/authentication/unsloth-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- LLM Fine-Tuning
- Machine Learning
- Open Source
- Reinforcement Learning
- Quantization
- Local AI
- Developer Tools
---
