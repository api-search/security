---
api_key_in: []
api_specs:
- filename: wombo-wai-openapi.yml
  format: yaml
  label: w.ai Inference API
  slug: wai-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wombo/refs/heads/main/openapi/wombo-wai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Wombo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wombo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wombo
provider_slug: wombo
scheme_count: 1
schemes:
- bearerFormat: wsk
  description: 'Developer API key issued at https://app.w.ai/developers/keys , sent as `Authorization: Bearer wsk-...`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wombo-wai-openapi.yml
  type: http
slug: wombo-authentication
source_filename: wombo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/wombo-wai-openapi.yml\ndocs: https://docs.w.ai/w.ai-api/api-features\nnotes: >-\n  Single auth model: a developer API key (prefix `wsk-`) generated at\n  https://app.w.ai/developers/keys and sent as an `Authorization: Bearer`\n  header on the OpenAI-compatible endpoints. The `wai` CLI uses separate Auth\n  API keys (env `W_AI_API_KEY`) managed via `wai key list` / `wai revoke`. No\n  OAuth 2.0 / OIDC scope surface is documented, so no scopes/ artifact.\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: wsk\n  description: 'Developer API key issued at https://app.w.ai/developers/keys , sent as `Authorization:\n    Bearer wsk-...`.'\n  sources:\n  - openapi/wombo-wai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wombo/refs/heads/main/authentication/wombo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Inference
- LLM
- Image Generation
- Generative AI
- Decentralized Compute
- GPU
- OpenAI Compatible
---
