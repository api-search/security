---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Goodfire Authentication
name_suffix: Authentication
oauth_flows: []
overview: Goodfire secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Goodfire
provider_slug: goodfire
scheme_count: 1
schemes:
- description: 'Ember API key issued from the Goodfire platform (https://platform.goodfire.ai). Supplied to the SDK via the GOODFIRE_API_KEY environment variable / goodfire.Client(api_key=...) and sent as an Authorization: Bearer <key> header on the OpenAI-compatible endpoint.'
  in: header
  name: apiKey
  parameter: Authorization
  scheme: bearer
  sources:
  - github.com/goodfire-ai/goodfire-sdk
  type: apiKey
slug: goodfire-authentication
source_filename: goodfire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/goodfire-ai/goodfire-sdk\ndocs: https://github.com/goodfire-ai/goodfire-sdk\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_transport: bearer\n  oauth2_flows: []\n  notes: >-\n    No published OpenAPI spec; auth profile captured from the official goodfire-sdk README\n    and Ember quickstart. Ember exposes an OpenAI-compatible inference surface, so keys are\n    presented as a Bearer token in the Authorization header.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  scheme: bearer\n  parameter: Authorization\n  description: >-\n    Ember API key issued from the Goodfire platform (https://platform.goodfire.ai). Supplied\n    to the SDK via the GOODFIRE_API_KEY environment variable / goodfire.Client(api_key=...)\n    and sent as an Authorization: Bearer <key> header on the OpenAI-compatible endpoint.\n  sources: [github.com/goodfire-ai/goodfire-sdk]\nkey_issuance: https://platform.goodfire.ai\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodfire/refs/heads/main/authentication/goodfire-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Interpretability
- LLM
- Model Steering
- Inference
- Developer Tools
- Research
---
