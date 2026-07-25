---
api_key_in:
- header
api_specs:
- filename: replicas-analytics-api-openapi.yml
  format: yaml
  label: Replicas Analytics API
  slug: replicas-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicas/refs/heads/main/openapi/replicas-analytics-api-openapi.yml
- filename: replicas-api-keys-api-openapi.yml
  format: yaml
  label: Replicas API Keys API
  slug: replicas-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicas/refs/heads/main/openapi/replicas-api-keys-api-openapi.yml
- filename: replicas-automation-api-openapi.yml
  format: yaml
  label: Replicas Automation API
  slug: replicas-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicas/refs/heads/main/openapi/replicas-automation-api-openapi.yml
- filename: replicas-credentials-api-openapi.yml
  format: yaml
  label: Replicas Credentials API
  slug: replicas-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicas/refs/heads/main/openapi/replicas-credentials-api-openapi.yml
- filename: replicas-downloads-api-openapi.yml
  format: yaml
  label: Replicas Downloads API
  slug: replicas-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicas/refs/heads/main/openapi/replicas-downloads-api-openapi.yml
- filename: replicas-environments-api-openapi.yml
  format: yaml
  label: Replicas Environments API
  slug: replicas-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicas/refs/heads/main/openapi/replicas-environments-api-openapi.yml
- filename: replicas-google-search-console-api-openapi.yml
  format: yaml
  label: Replicas Google Search Console API
  slug: replicas-google-search-console-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicas/refs/heads/main/openapi/replicas-google-search-console-api-openapi.yml
- filename: replicas-preview-api-openapi.yml
  format: yaml
  label: Replicas Preview API
  slug: replicas-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicas/refs/heads/main/openapi/replicas-preview-api-openapi.yml
- filename: replicas-profile-api-openapi.yml
  format: yaml
  label: Replicas Profile API
  slug: replicas-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicas/refs/heads/main/openapi/replicas-profile-api-openapi.yml
- filename: replicas-replica-api-openapi.yml
  format: yaml
  label: Replicas Replica API
  slug: replicas-replica-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicas/refs/heads/main/openapi/replicas-replica-api-openapi.yml
- filename: replicas-repository-api-openapi.yml
  format: yaml
  label: Replicas Repository API
  slug: replicas-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicas/refs/heads/main/openapi/replicas-repository-api-openapi.yml
- filename: replicas-slack-api-openapi.yml
  format: yaml
  label: Replicas Slack API
  slug: replicas-slack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicas/refs/heads/main/openapi/replicas-slack-api-openapi.yml
- filename: replicas-terminal-api-openapi.yml
  format: yaml
  label: Replicas Terminal API
  slug: replicas-terminal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicas/refs/heads/main/openapi/replicas-terminal-api-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Replicas Authentication
name_suffix: Authentication
oauth_flows: []
overview: Replicas secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Replicas
provider_slug: replicas
scheme_count: 3
schemes:
- applied_globally: true
  description: 'Primary API-key authentication. Obtain your API key from the Replicas dashboard under Organization -> Settings -> API Keys. Sent as Authorization: Bearer sk_replicas_...'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/replicas-openapi-original.json
  type: http
- description: Workspace engine secret used by agent-mode workspace requests, paired with the X-Workspace-Id header.
  name: engineSecret
  scheme: bearer
  sources:
  - openapi/replicas-openapi-original.json
  type: http
- description: Workspace ID used with the engine secret for agent-mode workspace requests.
  in: header
  name: workspaceId
  parameter: X-Workspace-Id
  sources:
  - openapi/replicas-openapi-original.json
  type: apiKey
slug: replicas-authentication
source_filename: replicas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/replicas-openapi-original.json\ndocs: https://docs.tryreplicas.com/features/api\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  model: >-\n    Bearer API-key authentication. Organization admins mint org-scoped API keys\n    (Organization -> Settings -> API Keys); any member can mint a personal API\n    key scoped to the user. Keys use the prefix `sk_replicas_...` and are sent as\n    `Authorization: Bearer <key>`. Agent-mode workspace requests use a separate\n    workspace engine secret (bearer) paired with an `X-Workspace-Id` header. One\n    automation trigger endpoint (fire custom webhook) is intentionally\n    unauthenticated - the URL token is the secret.\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: >-\n    Primary API-key authentication. Obtain your API key from the Replicas\n    dashboard under Organization -> Settings -> API Keys. Sent as\n    Authorization:\
  \ Bearer sk_replicas_...\n  applied_globally: true\n  sources:\n  - openapi/replicas-openapi-original.json\n- name: engineSecret\n  type: http\n  scheme: bearer\n  description: >-\n    Workspace engine secret used by agent-mode workspace requests, paired with\n    the X-Workspace-Id header.\n  sources:\n  - openapi/replicas-openapi-original.json\n- name: workspaceId\n  type: apiKey\n  in: header\n  parameter: X-Workspace-Id\n  description: Workspace ID used with the engine secret for agent-mode workspace requests.\n  sources:\n  - openapi/replicas-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replicas/refs/heads/main/authentication/replicas-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Company
- AI
- Coding Agents
- Developer Tools
- Automation
- Cloud Workspaces
- MCP
- DevOps
---
