---
anonymous_access: false
api_key_in: []
api_specs:
- filename: meetdarwin-ai-agent-api-openapi.yml
  format: yaml
  label: Darwin Agent API
  slug: meetdarwin-ai-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetdarwin-ai/openapi/meetdarwin-ai-agent-api-openapi.yml
- filename: meetdarwin-ai-analytics-api-openapi.yml
  format: yaml
  label: Darwin Analytics API
  slug: meetdarwin-ai-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetdarwin-ai/openapi/meetdarwin-ai-analytics-api-openapi.yml
- filename: meetdarwin-ai-chat-api-openapi.yml
  format: yaml
  label: Darwin Chat API
  slug: meetdarwin-ai-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetdarwin-ai/openapi/meetdarwin-ai-chat-api-openapi.yml
- filename: meetdarwin-ai-contacts-api-openapi.yml
  format: yaml
  label: Darwin Contacts API
  slug: meetdarwin-ai-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetdarwin-ai/openapi/meetdarwin-ai-contacts-api-openapi.yml
- filename: meetdarwin-ai-conversations-api-openapi.yml
  format: yaml
  label: Darwin Conversations API
  slug: meetdarwin-ai-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetdarwin-ai/openapi/meetdarwin-ai-conversations-api-openapi.yml
- filename: meetdarwin-ai-events-api-openapi.yml
  format: yaml
  label: Darwin Events API
  slug: meetdarwin-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetdarwin-ai/openapi/meetdarwin-ai-events-api-openapi.yml
- filename: meetdarwin-ai-experiments-api-openapi.yml
  format: yaml
  label: Darwin Experiments API
  slug: meetdarwin-ai-experiments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetdarwin-ai/openapi/meetdarwin-ai-experiments-api-openapi.yml
- filename: meetdarwin-ai-greetings-api-openapi.yml
  format: yaml
  label: Darwin Greetings API
  slug: meetdarwin-ai-greetings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetdarwin-ai/openapi/meetdarwin-ai-greetings-api-openapi.yml
- filename: meetdarwin-ai-knowledge-api-openapi.yml
  format: yaml
  label: Darwin Knowledge API
  slug: meetdarwin-ai-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetdarwin-ai/openapi/meetdarwin-ai-knowledge-api-openapi.yml
- filename: meetdarwin-ai-meetings-api-openapi.yml
  format: yaml
  label: Darwin Meetings API
  slug: meetdarwin-ai-meetings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetdarwin-ai/openapi/meetdarwin-ai-meetings-api-openapi.yml
- filename: meetdarwin-ai-outcomes-api-openapi.yml
  format: yaml
  label: Darwin Outcomes API
  slug: meetdarwin-ai-outcomes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetdarwin-ai/openapi/meetdarwin-ai-outcomes-api-openapi.yml
- filename: meetdarwin-ai-personal-links-api-openapi.yml
  format: yaml
  label: Darwin Personal links API
  slug: meetdarwin-ai-personal-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetdarwin-ai/openapi/meetdarwin-ai-personal-links-api-openapi.yml
- filename: meetdarwin-ai-privacy-api-openapi.yml
  format: yaml
  label: Darwin Privacy API
  slug: meetdarwin-ai-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetdarwin-ai/openapi/meetdarwin-ai-privacy-api-openapi.yml
- filename: meetdarwin-ai-webhooks-api-openapi.yml
  format: yaml
  label: Darwin Webhooks API
  slug: meetdarwin-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetdarwin-ai/openapi/meetdarwin-ai-webhooks-api-openapi.yml
- filename: meetdarwin-ai-workspace-api-openapi.yml
  format: yaml
  label: Darwin Workspace API
  slug: meetdarwin-ai-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetdarwin-ai/openapi/meetdarwin-ai-workspace-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Darwin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Darwin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Darwin
provider_slug: meetdarwin-ai
scheme_count: 1
schemes:
- description: 'A secret key (dk_live_…). Scopes: conversations:read, contacts:read, contacts:write, meetings:read, analytics:read, events:read, webhooks:write, knowledge:read, knowledge:write, agent:read, agent:write, experiments:read, experiments:write, privacy:write, chat:write.'
  name: bearer
  scheme: bearer
  sources:
  - openapi/meetdarwin-ai-mcp-openapi.json
  - openapi/meetdarwin-ai-openapi.json
  type: http
slug: meetdarwin-ai-authentication
source_filename: meetdarwin-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/meetdarwin-ai-mcp-openapi.json, openapi/meetdarwin-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'A secret key (dk_live_…). Scopes: conversations:read, contacts:read, contacts:write,\n    meetings:read, analytics:read, events:read, webhooks:write, knowledge:read, knowledge:write,\n    agent:read, agent:write, experiments:read, experiments:write, privacy:write, chat:write.'\n  sources:\n  - openapi/meetdarwin-ai-mcp-openapi.json\n  - openapi/meetdarwin-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/meetdarwin-ai/authentication/meetdarwin-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Sales
- Marketing
- Automation
- Conversational AI
---
