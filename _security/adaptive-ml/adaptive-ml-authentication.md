---
api_key_in:
- header
api_specs:
- filename: adaptive-ml-openapi-original.json
  format: json
  label: Adaptive Engine API
  slug: adaptive-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adaptive-ml/refs/heads/main/openapi/adaptive-ml-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Adaptive Ml Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adaptive ML secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Adaptive ML
provider_slug: adaptive-ml
scheme_count: 1
schemes:
- description: Personal or service-account API key. Generate a personal key from the project switcher (Generate new API key); create service accounts via adaptive.users.create_service_account for CI/CD and automation. The key is shown once at creation and cannot be retrieved later. Because the API is OpenAI-compatible, the OpenAI client authenticates the same way (api_key=ADAPTIVE_API_KEY, base_url=ADAPTIVE_URL/api/v1).
  env:
  - ADAPTIVE_URL
  - ADAPTIVE_API_KEY
  format: 'Authorization: Bearer <ADAPTIVE_API_KEY>'
  header: Authorization
  in: header
  name: bearerApiKey
  scheme: bearer
  sources:
  - docs
  type: http
slug: adaptive-ml-authentication
source_filename: adaptive-ml-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.adaptive-ml.com/v0.14/advanced/authentication\ndocs: https://docs.adaptive-ml.com/v0.14/advanced/authentication\nsummary:\n  types: [http]\n  http_scheme: bearer\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    Adaptive Engine is self-hosted; each deployment issues personal and\n    service-account API keys. Requests authenticate with a Bearer API key\n    against the deployment base URL (ADAPTIVE_URL). SSO/OIDC is available for\n    human user login to the console (not for API request auth).\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer <ADAPTIVE_API_KEY>'\n  env:\n  - ADAPTIVE_URL\n  - ADAPTIVE_API_KEY\n  sources: [docs]\n  description: >-\n    Personal or service-account API key. Generate a personal key from the\n    project switcher (Generate new API key); create service accounts via\n    adaptive.users.create_service_account\
  \ for CI/CD and automation. The key is\n    shown once at creation and cannot be retrieved later. Because the API is\n    OpenAI-compatible, the OpenAI client authenticates the same way\n    (api_key=ADAPTIVE_API_KEY, base_url=ADAPTIVE_URL/api/v1).\nsso:\n  protocol: oidc\n  scope: console-user-login-only\n  docs: https://docs.adaptive-ml.com/v0.14/advanced/sso\n  note: OIDC identity providers configure human login to the Adaptive console; not an API auth surface.\nnote: >-\n  The published OpenAPI (concorde) declares no components.securitySchemes; this\n  profile is searched from the docs auth page rather than derived from the spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaptive-ml/refs/heads/main/authentication/adaptive-ml-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai Ml
- LLM
- Fine-Tuning
- Reinforcement Learning
- Model Evaluation
- Inference
- OpenAI-Compatible
- MLOps
---
