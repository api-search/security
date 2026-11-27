---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cqnce-app-agents-admin-api-openapi.yml
  format: yaml
  label: cQnce Agents – Admin API
  slug: cqnce-app-agents-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-agents-admin-api-openapi.yml
- filename: cqnce-app-agents-self-api-openapi.yml
  format: yaml
  label: cQnce Agents – Self API
  slug: cqnce-app-agents-self-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-agents-self-api-openapi.yml
- filename: cqnce-app-alarms-api-openapi.yml
  format: yaml
  label: cQnce Alarms API
  slug: cqnce-app-alarms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-alarms-api-openapi.yml
- filename: cqnce-app-auth-agent-api-openapi.yml
  format: yaml
  label: cQnce Auth – Agent API
  slug: cqnce-app-auth-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-auth-agent-api-openapi.yml
- filename: cqnce-app-auth-tenant-api-openapi.yml
  format: yaml
  label: cQnce Auth – Tenant API
  slug: cqnce-app-auth-tenant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-auth-tenant-api-openapi.yml
- filename: cqnce-app-callbacks-api-openapi.yml
  format: yaml
  label: cQnce Callbacks API
  slug: cqnce-app-callbacks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-callbacks-api-openapi.yml
- filename: cqnce-app-health-api-openapi.yml
  format: yaml
  label: cQnce Health API
  slug: cqnce-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-health-api-openapi.yml
- filename: cqnce-app-logs-api-openapi.yml
  format: yaml
  label: cQnce Logs API
  slug: cqnce-app-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-logs-api-openapi.yml
- filename: cqnce-app-projects-api-openapi.yml
  format: yaml
  label: cQnce Projects API
  slug: cqnce-app-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-projects-api-openapi.yml
- filename: cqnce-app-public-api-openapi.yml
  format: yaml
  label: cQnce Public API
  slug: cqnce-app-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-public-api-openapi.yml
- filename: cqnce-app-requests-api-openapi.yml
  format: yaml
  label: cQnce Requests API
  slug: cqnce-app-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-requests-api-openapi.yml
- filename: cqnce-app-routing-rules-api-openapi.yml
  format: yaml
  label: cQnce Routing Rules API
  slug: cqnce-app-routing-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-routing-rules-api-openapi.yml
- filename: cqnce-app-subscriptions-api-openapi.yml
  format: yaml
  label: cQnce Subscriptions API
  slug: cqnce-app-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-subscriptions-api-openapi.yml
- filename: cqnce-app-teams-api-openapi.yml
  format: yaml
  label: cQnce Teams API
  slug: cqnce-app-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-teams-api-openapi.yml
- filename: cqnce-app-users-api-openapi.yml
  format: yaml
  label: cQnce Users API
  slug: cqnce-app-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-users-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: cQnce Authentication
name_suffix: Authentication
oauth_flows: []
overview: cQnce secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: cQnce
provider_slug: cqnce-app
scheme_count: 4
schemes:
- description: Per-project API key used for server-to-server request submission (e.g. POST /v1/requests). Docs - "Project API key (x-api-key header) for request submission endpoints such as /v1/requests."
  in: header
  name: projectApiKey
  parameter: x-api-key
  sources:
  - openapi/cqnce-app-openapi.yml
  - https://cqnce.app/en/developers
  type: apiKey
- bearerFormat: JWT
  description: Tenant JWT (Bearer) for management endpoints (projects, agents, teams, routing rules), obtained via POST /v1/auth/login.
  name: tenantJWT
  scheme: bearer
  sources:
  - openapi/cqnce-app-openapi.yml
  - https://cqnce.app/en/developers
  type: http
- bearerFormat: JWT
  description: JWT issued on agent login/register (POST /v1/auth/agent/login or /register); used by the approver mobile app surface.
  name: agentJWT
  scheme: bearer
  sources:
  - openapi/cqnce-app-openapi.yml
  type: http
- description: Optional client credentials headers (x-client-id, x-client-secret) are also supported for request submission flows. Not declared as a securityScheme in the OpenAPI; documented on the quickstart and SDK README.
  in: header
  name: clientCredentials
  parameter: x-client-id + x-client-secret
  sources:
  - https://cqnce.app/en/developers
  - https://github.com/cqnce-app/cqnce-sdk
  type: apiKey
slug: cqnce-app-authentication
source_filename: cqnce-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cqnce.app/en/developers\ndocs: https://cqnce.app/en/developers\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: projectApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Per-project API key used for server-to-server request submission (e.g. POST /v1/requests). Docs - \"Project API key (x-api-key header) for request submission endpoints such as /v1/requests.\"\n  sources:\n  - openapi/cqnce-app-openapi.yml\n  - https://cqnce.app/en/developers\n- name: tenantJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Tenant JWT (Bearer) for management endpoints (projects, agents, teams, routing rules), obtained via POST /v1/auth/login.\n  sources:\n  - openapi/cqnce-app-openapi.yml\n  - https://cqnce.app/en/developers\n- name: agentJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT issued on agent login/register (POST\
  \ /v1/auth/agent/login or /register); used by the approver mobile app surface.\n  sources:\n  - openapi/cqnce-app-openapi.yml\n- name: clientCredentials\n  type: apiKey\n  in: header\n  parameter: x-client-id + x-client-secret\n  description: Optional client credentials headers (x-client-id, x-client-secret) are also supported for request submission flows. Not declared as a securityScheme in the OpenAPI; documented on the quickstart and SDK README.\n  sources:\n  - https://cqnce.app/en/developers\n  - https://github.com/cqnce-app/cqnce-sdk\noauth2: false\nnote: No OAuth 2.0 / OIDC is documented; scopes artifact not applicable. Webhook callbacks are signed with HMAC-SHA256 (X-cQnce-Signature header) and decisions with ECDSA P-256.\n"
source_yaml_url: https://artifacts.apis.io/cqnce-app/authentication/cqnce-app-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Human-in-the-Loop
- Approvals
- Authorization
- AI Agents
- MCP
- Webhook
- Workflows
- Audit
---
