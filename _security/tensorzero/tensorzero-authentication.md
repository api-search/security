---
api_key_in:
- header
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tensorzero Authentication
name_suffix: Authentication
oauth_flows: []
overview: TensorZero secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TensorZero
provider_slug: tensorzero
scheme_count: 2
schemes:
- description: 'Optional client credential presented to the gateway (OpenAI-compatible Authorization: Bearer <token>). Enforced only when the operator sets up auth; disabled by default.'
  in: header
  name: bearerToken
  parameter: Authorization
  scheme: bearer
  sources:
  - docs
  type: http
- description: Upstream LLM-provider API keys (Anthropic, OpenAI, AWS Bedrock, Azure, GCP Vertex, Mistral, etc.) configured on the gateway via environment / configuration, never exposed to clients.
  in: header
  name: providerApiKeys
  sources:
  - docs
  type: apiKey
slug: tensorzero-authentication
source_filename: tensorzero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/tensorzero/tensorzero/tree/main/docs\ndocs: https://www.tensorzero.com/docs/operations/set-up-auth-for-tensorzero\nnotes: >-\n  TensorZero is a self-hosted gateway; there is no provider-hosted OpenAPI spec\n  to derive a security scheme from, so this profile is captured from the docs.\n  By default the gateway trusts its network boundary (no auth). Operators can\n  optionally enable authentication so clients access models without sharing the\n  underlying provider API keys. Because the gateway exposes an OpenAI-compatible\n  surface (POST /openai/v1/chat/completions), clients authenticate the same way\n  they would with OpenAI — a bearer token in the Authorization header — while\n  the gateway holds the real upstream provider credentials.\nsummary:\n  types: [http, apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    in: header\n   \
  \ parameter: Authorization\n    description: >-\n      Optional client credential presented to the gateway (OpenAI-compatible\n      Authorization: Bearer <token>). Enforced only when the operator sets up\n      auth; disabled by default.\n    sources: [docs]\n  - name: providerApiKeys\n    type: apiKey\n    in: header\n    description: >-\n      Upstream LLM-provider API keys (Anthropic, OpenAI, AWS Bedrock, Azure,\n      GCP Vertex, Mistral, etc.) configured on the gateway via environment /\n      configuration, never exposed to clients.\n    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tensorzero/refs/heads/main/authentication/tensorzero-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Ai Ml
- LLM
- LLMOps
- AI Gateway
- Inference
- Observability
- Open Source
- Model Routing
---
