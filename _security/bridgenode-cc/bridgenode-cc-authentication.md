---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: bridgenode-cc-models-api-openapi.yml
  format: yaml
  label: BridgeNode Models API
  slug: bridgenode-cc-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bridgenode-cc/openapi/bridgenode-cc-models-api-openapi.yml
- filename: bridgenode-cc-chat-completions-api-openapi.yml
  format: yaml
  label: BridgeNode Chat Completions API
  slug: bridgenode-cc-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bridgenode-cc/openapi/bridgenode-cc-chat-completions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: BridgeNode Authentication
name_suffix: Authentication
oauth_flows: []
overview: BridgeNode secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BridgeNode
provider_slug: bridgenode-cc
scheme_count: 1
schemes:
- in: header
  name: x402
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/bridgenode-cc-openapi.json
  type: apiKey
slug: bridgenode-cc-authentication
source_filename: bridgenode-cc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/bridgenode-cc-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  sources:\n  - openapi/bridgenode-cc-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/bridgenode-cc/authentication/bridgenode-cc-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Inference
- Payments
- Solana
- OpenAI-Compatible
---
