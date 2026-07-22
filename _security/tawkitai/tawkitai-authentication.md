---
api_key_in:
- header
- config
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tawkitai Authentication
name_suffix: Authentication
oauth_flows: []
overview: TawkitAI secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TawkitAI
provider_slug: tawkitai
scheme_count: 2
schemes:
- description: Copilot Cloud public API key passed to the frontend CopilotKit provider (publicApiKey prop) to connect an app to a hosted Copilot Cloud project.
  in: config
  name: copilotCloudPublicApiKey
  sources:
  - https://docs.copilotkit.ai/auth
  type: apiKey
- description: Self-managed Copilot Runtime deployments authenticate with whatever application-level auth the developer places in front of the runtime endpoint; no CopilotKit-imposed scheme.
  name: selfHostedRuntime
  sources:
  - https://docs.copilotkit.ai/backend/self-managed-agents
  type: custom
slug: tawkitai-authentication
source_filename: tawkitai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.copilotkit.ai/auth\ndocs: https://docs.copilotkit.ai/auth\nsummary:\n  types: [apiKey]\n  api_key_in: [header, config]\n  oauth2_flows: []\nnote: >-\n  CopilotKit is a framework rather than a REST provider, so there is no OpenAPI\n  securitySchemes block to derive from. Copilot Cloud is authenticated with a\n  project API key: a public API key is supplied to the frontend <CopilotKit>\n  provider (publicApiKey), and requests are routed through the hosted Copilot\n  Runtime. Self-hosted deployments run their own Copilot Runtime and can layer\n  arbitrary application auth in front of it.\nschemes:\n  - name: copilotCloudPublicApiKey\n    type: apiKey\n    in: config\n    description: >-\n      Copilot Cloud public API key passed to the frontend CopilotKit provider\n      (publicApiKey prop) to connect an app to a hosted Copilot Cloud project.\n    sources: [https://docs.copilotkit.ai/auth]\n  - name: selfHostedRuntime\n\
  \    type: custom\n    description: >-\n      Self-managed Copilot Runtime deployments authenticate with whatever\n      application-level auth the developer places in front of the runtime\n      endpoint; no CopilotKit-imposed scheme.\n    sources: [https://docs.copilotkit.ai/backend/self-managed-agents]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tawkitai/refs/heads/main/authentication/tawkitai-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- AI Agents
- Copilots
- Generative UI
- Frontend
- Developer Tools
- React
- SDK
- Open Source
- LLM
---
