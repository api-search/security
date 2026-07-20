---
api_key_in: []
api_specs:
- filename: boom-ai-openapi-original.json
  format: json
  label: Boom API
  slug: boom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Boom Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boom Ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Boom Ai
provider_slug: boom-ai
scheme_count: 1
schemes:
- description: 'Organization API key, sent as `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/boom-ai-openapi-original.json
  type: http
slug: boom-ai-authentication
source_filename: boom-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/boom-ai-openapi-original.json\ndocs: https://docs.useboom.ai/quickstart\nnotes: >-\n  Single scheme: a per-organization Bearer API key with the prefix `boom_org_...`,\n  sent as `Authorization: Bearer <key>`. Applied globally to every operation. Use a\n  development-organization key against the https://dev.useboom.ai sandbox host. The\n  hosted MCP server authenticates instead via interactive Boom dashboard login (OAuth),\n  not the API key. No OAuth2 scopes surface — access is scoped to the organization and\n  destructive actions require an org admin.\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Organization API key, sent as `Authorization: Bearer [example key]`.'\n  sources:\n  - openapi/boom-ai-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/authentication/boom-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Conversational AI
- Customer Engagement
- Customer Data Platform
- Messaging
- WhatsApp
- SMS
- Marketing Automation
- E-commerce
- Agents
- MCP
---
