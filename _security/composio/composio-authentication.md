---
api_key_in:
- cookie
- header
api_specs:
- filename: composio-auth-configs-api-openapi.yml
  format: yaml
  label: Composio Auth Configs API
  slug: composio-auth-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-auth-configs-api-openapi.yml
- filename: composio-authentication-api-openapi.yml
  format: yaml
  label: Composio Authentication API
  slug: composio-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-authentication-api-openapi.yml
- filename: composio-cli-api-openapi.yml
  format: yaml
  label: Composio CLI API
  slug: composio-cli-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-cli-api-openapi.yml
- filename: composio-cli-authentication-api-openapi.yml
  format: yaml
  label: Composio CLI Authentication API
  slug: composio-cli-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-cli-authentication-api-openapi.yml
- filename: composio-connected-accounts-api-openapi.yml
  format: yaml
  label: Composio Connected Accounts API
  slug: composio-connected-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-connected-accounts-api-openapi.yml
- filename: composio-files-api-openapi.yml
  format: yaml
  label: Composio Files API
  slug: composio-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-files-api-openapi.yml
- filename: composio-logs-api-openapi.yml
  format: yaml
  label: Composio Logs API
  slug: composio-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-logs-api-openapi.yml
- filename: composio-mcp-api-openapi.yml
  format: yaml
  label: Composio MCP API
  slug: composio-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-mcp-api-openapi.yml
- filename: composio-migration-api-openapi.yml
  format: yaml
  label: Composio Migration API
  slug: composio-migration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-migration-api-openapi.yml
- filename: composio-organization-management-api-openapi.yml
  format: yaml
  label: Composio Organization Management API
  slug: composio-organization-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-organization-management-api-openapi.yml
- filename: composio-projects-api-openapi.yml
  format: yaml
  label: Composio Projects API
  slug: composio-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-projects-api-openapi.yml
- filename: composio-tool-router-api-openapi.yml
  format: yaml
  label: Composio Tool Router API
  slug: composio-tool-router-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-tool-router-api-openapi.yml
- filename: composio-toolkits-api-openapi.yml
  format: yaml
  label: Composio Toolkits API
  slug: composio-toolkits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-toolkits-api-openapi.yml
- filename: composio-tools-api-openapi.yml
  format: yaml
  label: Composio Tools API
  slug: composio-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-tools-api-openapi.yml
- filename: composio-triggers-api-openapi.yml
  format: yaml
  label: Composio Triggers API
  slug: composio-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-triggers-api-openapi.yml
- filename: composio-webhook-endpoints-api-openapi.yml
  format: yaml
  label: Composio Webhook Endpoints API
  slug: composio-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-webhook-endpoints-api-openapi.yml
- filename: composio-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Composio Webhook Subscriptions API
  slug: composio-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/openapi/composio-webhook-subscriptions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Composio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Composio secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Composio
provider_slug: composio
scheme_count: 4
schemes:
- description: Project API key authentication
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/composio-openapi-original.json
  - openapi/composio-openapi-original.yml
  type: apiKey
- description: User API key authentication
  in: header
  name: UserApiKeyAuth
  parameter: x-user-api-key
  sources:
  - openapi/composio-openapi-original.json
  type: apiKey
- description: Cookie-based session authentication
  in: cookie
  name: CookieAuth
  parameter: authToken
  sources:
  - openapi/composio-openapi-original.json
  type: apiKey
- description: Organization API key authentication
  in: header
  name: OrgApiKeyAuth
  parameter: x-org-api-key
  sources:
  - openapi/composio-openapi-original.json
  type: apiKey
slug: composio-authentication
source_filename: composio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/composio-openapi-original.json, openapi/composio-openapi-original.yml\ndocs: https://docs.composio.dev/faq/api_key/api_key\nnotes: >-\n  The Composio platform API is API-key authenticated (project, user, and org keys via\n  header, plus a cookie session for the dashboard). API keys can carry scoped\n  permissions (e.g. MCP, files, realtime routes). Distinct from this, Composio manages\n  OAuth2 flows on behalf of end users to connect third-party toolkits (delegated auth);\n  those tokens are held by Composio and never exposed to the agent, so they are not a\n  securityScheme on this API.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Project API key authentication\n  sources:\n  - openapi/composio-openapi-original.json\n  - openapi/composio-openapi-original.yml\n- name: UserApiKeyAuth\n  type:\
  \ apiKey\n  in: header\n  parameter: x-user-api-key\n  description: User API key authentication\n  sources:\n  - openapi/composio-openapi-original.json\n- name: CookieAuth\n  type: apiKey\n  in: cookie\n  parameter: authToken\n  description: Cookie-based session authentication\n  sources:\n  - openapi/composio-openapi-original.json\n- name: OrgApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-org-api-key\n  description: Organization API key authentication\n  sources:\n  - openapi/composio-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/authentication/composio-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- AI Agents
- Authentication
- Integration
- MCP
- Sandbox
- Tools
- Triggers
- Unified_API
- Webhook
---
