---
api_key_in:
- client-constructor
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Ashr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ashr secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ashr
provider_slug: ashr
scheme_count: 1
schemes:
- description: Ashr Labs authenticates with a secret API key issued in the Ashr Labs console (lab.ashr.io). Keys carry a "tp_" prefix and are passed to the SDK client constructor, e.g. AshrLabsClient(api_key="tp_...") in the Python SDK and the equivalent in the TypeScript SDK. The SDK setup validates the key before scaffolding and running evals.
  in: client-constructor
  key_prefix: tp_
  name: apiKey
  sources:
  - https://ashr.io/docs/python-sdk/overview/
  type: apiKey
slug: ashr-authentication
source_filename: ashr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://ashr.io/docs/python-sdk/overview/\ndocs: https://ashr.io/docs/python-sdk/overview/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - client-constructor\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: apiKey\n  description: >-\n    Ashr Labs authenticates with a secret API key issued in the Ashr Labs\n    console (lab.ashr.io). Keys carry a \"tp_\" prefix and are passed to the SDK\n    client constructor, e.g. AshrLabsClient(api_key=\"tp_...\") in the Python SDK\n    and the equivalent in the TypeScript SDK. The SDK setup validates the key\n    before scaffolding and running evals.\n  key_prefix: tp_\n  in: client-constructor\n  sources:\n  - https://ashr.io/docs/python-sdk/overview/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ashr/refs/heads/main/authentication/ashr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- AI Agents
- Agent Testing
- Evaluation
- Observability
- LLM
- Developer Tools
- SDK
---
