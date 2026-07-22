---
api_key_in: []
auth_types:
- provider-api-key
- sso
description: ''
kind: authentication
layout: security
method: searched
name: Flow Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flow AI secures its APIs with provider-api-key and sso across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Flow AI
provider_slug: flow-ai
scheme_count: 2
schemes:
- example_names:
  - ANTHROPIC_API_KEY
  in: env
  location: environment variables / runtime config
  name: model-provider-keys
  scope: model provider access for live runs
  sources:
  - https://flow-ai.com/docs
  type: apiKey
- capabilities:
  - SSO
  - RBAC
  - credential-vault
  name: studio-sso
  sources:
  - https://flow-ai.com/pricing
  tier: production
  type: sso
slug: flow-ai-authentication
source_filename: flow-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://flow-ai.com/docs\nsummary:\n  model: bring-your-own-keys\n  types:\n  - provider-api-key\n  - sso\n  notes: >-\n    flowai-harness runs inside the host's own infrastructure, so there is no\n    Flow-AI-issued end-user API credential. Agents authenticate to model providers\n    with the host's own keys (e.g. ANTHROPIC_API_KEY, OpenAI, Bedrock, Azure,\n    Vertex) supplied via environment/config, and to warehouses with the host's own\n    connection credentials. The Production tier adds multi-user Studio with SSO/RBAC\n    and a credential vault for managing those secrets.\nschemes:\n- name: model-provider-keys\n  type: apiKey\n  in: env\n  location: environment variables / runtime config\n  example_names:\n  - ANTHROPIC_API_KEY\n  scope: model provider access for live runs\n  sources:\n  - https://flow-ai.com/docs\n- name: studio-sso\n  type: sso\n  tier: production\n  capabilities:\n  - SSO\n  - RBAC\n  - credential-vault\n\
  \  sources:\n  - https://flow-ai.com/pricing\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flow-ai/refs/heads/main/authentication/flow-ai-authentication.yml
summary_line: provider-api-key/sso · 2 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agent Infrastructure
- LLM Evaluation
- Data
- Runtime
- SDK
- Model Context Protocol
- Analytics
---
