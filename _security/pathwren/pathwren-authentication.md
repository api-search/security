---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pathwren-bulk-api-openapi.yml
  format: yaml
  label: AI Crawler Index Bulk API
  slug: pathwren-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathwren/refs/heads/main/openapi/pathwren-bulk-api-openapi.yml
- filename: pathwren-crawlers-api-openapi.yml
  format: yaml
  label: AI Crawler Index Crawlers API
  slug: pathwren-crawlers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathwren/refs/heads/main/openapi/pathwren-crawlers-api-openapi.yml
- filename: pathwren-ip-ranges-api-openapi.yml
  format: yaml
  label: AI Crawler Index Ip Ranges API
  slug: pathwren-ip-ranges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathwren/refs/heads/main/openapi/pathwren-ip-ranges-api-openapi.yml
- filename: pathwren-robots-api-openapi.yml
  format: yaml
  label: AI Crawler Index Robots API
  slug: pathwren-robots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathwren/refs/heads/main/openapi/pathwren-robots-api-openapi.yml
- filename: pathwren-status-api-openapi.yml
  format: yaml
  label: AI Crawler Index Status API
  slug: pathwren-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathwren/refs/heads/main/openapi/pathwren-status-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Pathwren Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI Crawler Index declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: AI Crawler Index
provider_slug: pathwren
scheme_count: 0
schemes: []
slug: pathwren-authentication
source_filename: pathwren-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: https://www.pathwren.workers.dev/.well-known/api-onboarding\ndocs: https://www.pathwren.workers.dev/api.html\nsummary: >-\n  No authentication of any kind. The OpenAPI 3.1 document declares an empty\n  components.securitySchemes and no top-level security requirement; the provider's machine-readable\n  onboarding document states authentication.required=false, type \"none\", with the note \"There is no\n  key, no token, no signup and no account. Send the GET.\"\nschemes: []\nscheme_count: 0\nanonymous_access: true\nevidence:\n- kind: openapi\n  url: https://www.pathwren.workers.dev/openapi.json\n  detail: components.securitySchemes is empty; no security[] on any of the 68 operations.\n- kind: onboarding\n  url: https://www.pathwren.workers.dev/.well-known/api-onboarding\n  http_status: 200\n  detail: 'authentication: {required: false, type: none}'\n- kind: plugin-manifest\n  url: https://www.pathwren.workers.dev/.well-known/ai-plugin.json\n\
  \  http_status: 200\n  detail: 'auth: {type: none}; api.is_user_authenticated false'\n- kind: probe\n  url: https://www.pathwren.workers.dev/data/agents.json\n  http_status: 200\n  detail: Unauthenticated GET returned 200 with the full 74KB payload and Access-Control-Allow-Origin:*.\noauth:\n  present: false\n  detail: >-\n    Probed anonymously on 2026-09-01: /.well-known/oauth-authorization-server 404,\n    /.well-known/oauth-protected-resource 404, /.well-known/openid-configuration 404 — each with a\n    JSON body. The provider documents these as deliberate machine-readable refusals in\n    /.well-known/mcp.json (x-authorization): the servers never issue a 401 and never inspect an\n    Authorization header.\nmcp_authentication:\n  endpoints:\n  - https://www.pathwren.workers.dev/mcp\n  - https://www.pathwren.workers.dev/mcp/triage\n  - https://www.pathwren.workers.dev/mcp/doctor\n  required: false\n  verified: probed\n  detail: tools/list answered HTTP 200 on all three with no credential.\n\
  a2a_authentication:\n  endpoint: https://www.pathwren.workers.dev/a2a\n  required: false\n  detail: The agent card declares no securitySchemes and no security requirement.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pathwren/refs/heads/main/authentication/pathwren-authentication.yml
summary_line: 0 schemes
tags:
- AI crawlers
- web crawlers
- Robots.txt
- User Agents
- Bot Detection
- GPTBot
- ClaudeBot
- crawler IP ranges
- llms-txt
- Open Data
- A2A
---
