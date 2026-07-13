---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ai Gateway Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI Gateway secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AI Gateway
provider_slug: ai-gateway
scheme_count: 2
schemes:
- description: Portkey API key header.
  in: header
  name: PortkeyApiKey
  parameter: x-portkey-api-key
  sources:
  - openapi/ai-gateway-openapi.yml
  type: apiKey
- description: Upstream provider selector header.
  in: header
  name: PortkeyProvider
  parameter: x-portkey-provider
  sources:
  - openapi/ai-gateway-openapi.yml
  type: apiKey
slug: ai-gateway-authentication
source_filename: ai-gateway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ai-gateway-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: PortkeyApiKey\n  type: apiKey\n  in: header\n  parameter: x-portkey-api-key\n  description: Portkey API key header.\n  sources:\n  - openapi/ai-gateway-openapi.yml\n- name: PortkeyProvider\n  type: apiKey\n  in: header\n  parameter: x-portkey-provider\n  description: Upstream provider selector header.\n  sources:\n  - openapi/ai-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai-gateway/refs/heads/main/authentication/ai-gateway-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- AI Gateway
- LLM Router
- LLM Proxy
- Model Routing
- Prompt Firewall
- Guardrails
- AI Observability
- Cost Controls
- AI Governance
- API Gateway
---
