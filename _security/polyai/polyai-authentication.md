---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Polyai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Polyai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Polyai
provider_slug: polyai
scheme_count: 1
schemes:
- description: Region- and scope-provisioned API key. Sent on every request as the x-api-key header. Treat keys as secrets; never commit or embed in client-side code.
  in: header
  name: apiKeyHeader
  parameter_name: x-api-key
  sources:
  - https://docs.poly.ai/api-reference/introduction
  type: apiKey
slug: polyai-authentication
source_filename: polyai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.poly.ai/api-reference/introduction\ndocs: https://docs.poly.ai/api-reference/introduction\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    All PolyAI Platform APIs use header-based API-key authentication. There is no\n    OAuth2/OIDC flow. Keys are region- and scope-specific (workspace-scoped for\n    Agents, project-scoped for Conversations) and must be created in the Agent\n    Studio \"API Keys\" tab. Runtime and build keys are separate. The Messaging\n    (WebSocket) API additionally exchanges a connector token for a short-lived\n    access token before opening a session.\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: >-\n    Region- and scope-provisioned API key. Sent on every request as the x-api-key\n    header. Treat keys as secrets; never commit or embed in client-side code.\n  sources: [https://docs.poly.ai/api-reference/introduction]\n\
  key_scopes:\n- {scope: workspace, used_by: Agents API, direction: write}\n- {scope: project, used_by: Conversations API, direction: read}\n- {scope: runtime, used_by: runtime conversation/chat surfaces}\n- {scope: build, used_by: agent build/monitoring surfaces}\nmessaging_token_exchange:\n  description: >-\n    The Messaging (WebSocket) API exchanges a connector token for a short-lived\n    access token, then creates a session before events flow.\n  source: https://docs.poly.ai/api-reference/messaging/sessions\ncorrelation:\n  response_header: X-PolyAI-Correlation-Id\n  description: Correlation/request id echoed on responses and surfaced as error_id on errors.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polyai/refs/heads/main/authentication/polyai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Conversational AI
- Voice AI
- Customer Service
- Contact Center
- Agents
- Speech Recognition
- Text to Speech
- Webhooks
- Enterprise
---
