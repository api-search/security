---
api_key_in: []
api_specs:
- filename: boom-ai-cdp-custom-objects-api-openapi.yml
  format: yaml
  label: Boom Ai CDP Custom Objects API
  slug: boom-ai-cdp-custom-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-cdp-custom-objects-api-openapi.yml
- filename: boom-ai-cdp-events-api-openapi.yml
  format: yaml
  label: Boom Ai CDP Events API
  slug: boom-ai-cdp-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-cdp-events-api-openapi.yml
- filename: boom-ai-cdp-people-api-openapi.yml
  format: yaml
  label: Boom Ai CDP People API
  slug: boom-ai-cdp-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-cdp-people-api-openapi.yml
- filename: boom-ai-cdp-relationships-api-openapi.yml
  format: yaml
  label: Boom Ai CDP Relationships API
  slug: boom-ai-cdp-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-cdp-relationships-api-openapi.yml
- filename: boom-ai-cdp-sources-api-openapi.yml
  format: yaml
  label: Boom Ai CDP Sources API
  slug: boom-ai-cdp-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-cdp-sources-api-openapi.yml
- filename: boom-ai-http-credentials-api-openapi.yml
  format: yaml
  label: Boom Ai HTTP credentials API
  slug: boom-ai-http-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-http-credentials-api-openapi.yml
- filename: boom-ai-initiatives-api-openapi.yml
  format: yaml
  label: Boom Ai Initiatives API
  slug: boom-ai-initiatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-initiatives-api-openapi.yml
- filename: boom-ai-journeys-api-openapi.yml
  format: yaml
  label: Boom Ai Journeys API
  slug: boom-ai-journeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-journeys-api-openapi.yml
- filename: boom-ai-segments-api-openapi.yml
  format: yaml
  label: Boom Ai Segments API
  slug: boom-ai-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-segments-api-openapi.yml
- filename: boom-ai-whatsapp-templates-api-openapi.yml
  format: yaml
  label: Boom Ai WhatsApp templates API
  slug: boom-ai-whatsapp-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-whatsapp-templates-api-openapi.yml
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
