---
api_key_in:
- header
- environment
auth_types:
- http-basic
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Lightningai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lightning.AI secures its APIs with http-basic and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lightning.AI
provider_slug: lightningai
scheme_count: 2
schemes:
- applies_to: Lightning AI Platform API (https://lightning.ai/api/v1), SDK and CLI
  credentials:
  - LIGHTNING_USER_ID
  - LIGHTNING_API_KEY
  headless: export LIGHTNING_USER_ID=... LIGHTNING_API_KEY=...
  interactive_login: lightning login
  name: platformBasicAuth
  scheme: basic
  source: https://lightning.ai/docs/platform/developers/cli
  type: http
- applies_to: Lightning Model APIs / LLM gateway (https://lightning.ai/v1)
  header: 'Authorization: Bearer <LIGHTNING_API_KEY>'
  key_console: https://lightning.ai/lightning-ai/model-apis/models?showApiKey=true
  key_management:
  - lightning api-key get [--org NAME]
  - lightning api-key create --org NAME --name my-key
  - lightning api-key list
  - lightning api-key delete <KEY_ID>
  name: modelApiBearer
  scheme: bearer
  scoping: Model-API keys are scoped to an organization; pass --org or set LIGHTNING_ORG when the user belongs to more than one org.
  type: http
  verified: GET https://lightning.ai/v1/models without a token returns 401 {"code":16,"message":"unauthenticated","details":[]}
slug: lightningai-authentication
source_filename: lightningai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://lightning.ai/docs/platform/developers/cli\ndocs:\n- https://lightning.ai/docs/platform/developers/cli\n- https://lightning.ai/docs/platform/inference/model-apis\n- https://github.com/Lightning-AI/skills/blob/main/lightning-llm-gateway/SKILL.md\nnotes: >-\n  Lightning AI runs TWO distinct auth schemes and its own docs warn not to conflate them.\n  Platform SDK/CLI/REST calls (Studios, Jobs, Deployments, Sandboxes) use HTTP Basic with\n  `LIGHTNING_USER_ID` as the user and `LIGHTNING_API_KEY` as the password — both are required.\n  The OpenAI-compatible Model APIs (LLM gateway) use a Bearer token minted separately via\n  `lightning api-key get`. No OAuth 2.0 or OpenID Connect surface is published: there is no\n  /.well-known/openid-configuration and no /.well-known/oauth-authorization-server (see\n  well-known/lightningai-well-known.yml), so there is no scopes/ artifact for this provider.\nsummary:\n  types: [http-basic,\
  \ http-bearer]\n  api_key_in: [header, environment]\n  oauth2_flows: []\nschemes:\n- name: platformBasicAuth\n  type: http\n  scheme: basic\n  applies_to: Lightning AI Platform API (https://lightning.ai/api/v1), SDK and CLI\n  credentials:\n  - LIGHTNING_USER_ID\n  - LIGHTNING_API_KEY\n  interactive_login: lightning login\n  headless: export LIGHTNING_USER_ID=... LIGHTNING_API_KEY=...\n  source: https://lightning.ai/docs/platform/developers/cli\n- name: modelApiBearer\n  type: http\n  scheme: bearer\n  applies_to: Lightning Model APIs / LLM gateway (https://lightning.ai/v1)\n  header: 'Authorization: Bearer <LIGHTNING_API_KEY>'\n  key_management:\n  - lightning api-key get [--org NAME]\n  - lightning api-key create --org NAME --name my-key\n  - lightning api-key list\n  - lightning api-key delete <KEY_ID>\n  key_console: https://lightning.ai/lightning-ai/model-apis/models?showApiKey=true\n  scoping: >-\n    Model-API keys are scoped to an organization; pass --org or set LIGHTNING_ORG when\
  \ the user\n    belongs to more than one org.\n  verified: >-\n    GET https://lightning.ai/v1/models without a token returns 401\n    {\"code\":16,\"message\":\"unauthenticated\",\"details\":[]}\nanonymous_endpoints:\n- method: GET\n  url: https://lightning.ai/api/v1/models\n  note: public OpenAI-style model catalog, returns 200 without credentials\n- method: GET\n  url: https://lightning.ai/api/v1/docs/worlds\n  note: public docs worlds registry, returns 200 without credentials\nrelated:\n- conventions/lightningai-conventions.yml\n- cli/lightningai-cli.yml\n- rate-limits/lightningai-rate-limits.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightningai/refs/heads/main/authentication/lightningai-authentication.yml
summary_line: http-basic/http-bearer · 2 schemes
tags:
- Company
- Ai Infrastructure
- Artificial Intelligence
- Machine Learning
- GPU Cloud
- Model Inference
- LLM Gateway
- Developer Tools
- MLOps
- Deployment
---
