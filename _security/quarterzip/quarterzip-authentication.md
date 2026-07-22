---
api_key_in:
- client-config
auth_types:
- workspace-token
- hmac-signature
description: ''
kind: authentication
layout: security
method: searched
name: Quarterzip Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quarterzip secures its APIs with workspace-token and hmac-signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Quarterzip
provider_slug: quarterzip
scheme_count: 2
schemes:
- description: Workspace token issued by Quarterzip (app Settings), passed to Quarterzip.open() together with an agentId (from the agent URL /w/{WORKSPACE_ID}/a/{AGENT_ID}).
  in: sdk-config
  name: workspaceToken
  source: https://docs.quarterzip.ai/sdk-api
  type: apiKey
- description: Inbound webhook deliveries are signed with an HMAC (Standard Webhooks) using the workspace signing secret; consumers verify the webhook-signature header.
  name: webhookSignature
  scheme: standard-webhooks
  secret_format: whsec_
  source: https://docs.quarterzip.ai/webhooks
  type: hmac
slug: quarterzip-authentication
source_filename: quarterzip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.quarterzip.ai/sdk-api\ndocs: https://docs.quarterzip.ai/sdk-api\nnote: >-\n  Quarterzip exposes a client-side JavaScript SDK and signed webhooks rather than a\n  traditional REST API. Authentication is derived from the published SDK and webhook\n  docs, not an OpenAPI securityScheme.\nsummary:\n  types:\n  - workspace-token\n  - hmac-signature\n  api_key_in:\n  - client-config\nschemes:\n- name: workspaceToken\n  type: apiKey\n  in: sdk-config\n  description: >-\n    Workspace token issued by Quarterzip (app Settings), passed to Quarterzip.open()\n    together with an agentId (from the agent URL /w/{WORKSPACE_ID}/a/{AGENT_ID}).\n  source: https://docs.quarterzip.ai/sdk-api\n- name: webhookSignature\n  type: hmac\n  scheme: standard-webhooks\n  secret_format: whsec_\n  description: >-\n    Inbound webhook deliveries are signed with an HMAC (Standard Webhooks) using the\n    workspace signing secret; consumers verify\
  \ the webhook-signature header.\n  source: https://docs.quarterzip.ai/webhooks\ncontrols:\n- domain-restriction: >-\n    Origin-header validation (\"domain restriction\") can be enabled in the Quarterzip\n    app so SDK requests are only accepted from allowlisted origins.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quarterzip/refs/heads/main/authentication/quarterzip-authentication.yml
summary_line: workspace-token/hmac-signature · 2 schemes
tags:
- Company
- AI Agents
- Customer Support
- Onboarding
- User Activation
- Screen Sharing
- Voice
- Webhooks
- SDK
- Developer Tools
---
