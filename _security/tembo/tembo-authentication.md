---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tembo-agents-api-openapi.yml
  format: yaml
  label: Tembo Agents API
  slug: tembo-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-agents-api-openapi.yml
- filename: tembo-api-keys-api-openapi.yml
  format: yaml
  label: Tembo API Keys API
  slug: tembo-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-api-keys-api-openapi.yml
- filename: tembo-artifacts-api-openapi.yml
  format: yaml
  label: Tembo Artifacts API
  slug: tembo-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-artifacts-api-openapi.yml
- filename: tembo-authentication-api-openapi.yml
  format: yaml
  label: Tembo Authentication API
  slug: tembo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-authentication-api-openapi.yml
- filename: tembo-billing-api-openapi.yml
  format: yaml
  label: Tembo Billing API
  slug: tembo-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-billing-api-openapi.yml
- filename: tembo-insights-api-openapi.yml
  format: yaml
  label: Tembo Insights API
  slug: tembo-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-insights-api-openapi.yml
- filename: tembo-integrations-api-openapi.yml
  format: yaml
  label: Tembo Integrations API
  slug: tembo-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-integrations-api-openapi.yml
- filename: tembo-mcp-connections-api-openapi.yml
  format: yaml
  label: Tembo MCP Connections API
  slug: tembo-mcp-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-mcp-connections-api-openapi.yml
- filename: tembo-messages-api-openapi.yml
  format: yaml
  label: Tembo Messages API
  slug: tembo-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-messages-api-openapi.yml
- filename: tembo-models-api-openapi.yml
  format: yaml
  label: Tembo Models API
  slug: tembo-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-models-api-openapi.yml
- filename: tembo-oauth-api-openapi.yml
  format: yaml
  label: Tembo OAuth API
  slug: tembo-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-oauth-api-openapi.yml
- filename: tembo-organizations-api-openapi.yml
  format: yaml
  label: Tembo Organizations API
  slug: tembo-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-organizations-api-openapi.yml
- filename: tembo-projects-api-openapi.yml
  format: yaml
  label: Tembo Projects API
  slug: tembo-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-projects-api-openapi.yml
- filename: tembo-pull-requests-api-openapi.yml
  format: yaml
  label: Tembo Pull requests API
  slug: tembo-pull-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-pull-requests-api-openapi.yml
- filename: tembo-repositories-api-openapi.yml
  format: yaml
  label: Tembo Repositories API
  slug: tembo-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-repositories-api-openapi.yml
- filename: tembo-runtimes-api-openapi.yml
  format: yaml
  label: Tembo Runtimes API
  slug: tembo-runtimes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-runtimes-api-openapi.yml
- filename: tembo-sessions-api-openapi.yml
  format: yaml
  label: Tembo Sessions API
  slug: tembo-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-sessions-api-openapi.yml
- filename: tembo-skills-api-openapi.yml
  format: yaml
  label: Tembo Skills API
  slug: tembo-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-skills-api-openapi.yml
- filename: tembo-users-api-openapi.yml
  format: yaml
  label: Tembo Users API
  slug: tembo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/openapi/tembo-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Tembo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tembo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tembo
provider_slug: tembo
scheme_count: 1
schemes:
- name: apiKey
  scheme: bearer
  sources:
  - openapi/tembo-openapi.yml
  type: http
slug: tembo-authentication
source_filename: tembo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/tembo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/tembo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tembo/refs/heads/main/authentication/tembo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI Agents
- Coding Agents
- Developer Tools
- Sandbox
- MCP
- Automation
---
