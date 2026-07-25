---
api_key_in:
- header
api_specs:
- filename: postman-webhooks-asyncapi.yml
  format: yaml
  label: Postman
  slug: postman
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/asyncapi/postman-webhooks-asyncapi.yml
- filename: postman-collections-api-openapi.yml
  format: yaml
  label: Postman Collections API
  slug: collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-collections-api-openapi.yml
- filename: postman-workspaces-api-openapi.yml
  format: yaml
  label: Postman Workspaces API
  slug: workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-workspaces-api-openapi.yml
- filename: postman-environments-api-openapi.yml
  format: yaml
  label: Postman Environments API
  slug: environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-environments-api-openapi.yml
- filename: postman-monitors-api-openapi.yml
  format: yaml
  label: Postman Monitors API
  slug: monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-monitors-api-openapi.yml
- filename: postman-apis-api-openapi.yml
  format: yaml
  label: Postman APIs / Spec Hub API
  slug: apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-apis-api-openapi.yml
- filename: postman-private-api-network-api-openapi.yml
  format: yaml
  label: Postman Private API Network API
  slug: private-api-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-private-api-network-api-openapi.yml
- filename: postman-webhooks-api-openapi.yml
  format: yaml
  label: Postman Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-webhooks-api-openapi.yml
- filename: postman-collection-runs-api-openapi.yml
  format: yaml
  label: Postman Collection Runs API
  slug: collection-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-collection-runs-api-openapi.yml
- filename: postman-tags-api-openapi.yml
  format: yaml
  label: Postman Tags API
  slug: tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-tags-api-openapi.yml
- filename: postman-audit-logs-api-openapi.yml
  format: yaml
  label: Postman Audit Logs API
  slug: audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-audit-logs-api-openapi.yml
- filename: postman-secret-scanner-api-openapi.yml
  format: yaml
  label: Postman Secret Scanner API
  slug: secret-scanner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-secret-scanner-api-openapi.yml
- filename: postman-api-comments-api-openapi.yml
  format: yaml
  label: Postman API Comments API
  slug: postman-api-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-api-comments-api-openapi.yml
- filename: postman-api-schemas-api-openapi.yml
  format: yaml
  label: Postman API Schemas API
  slug: postman-api-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-api-schemas-api-openapi.yml
- filename: postman-api-versions-api-openapi.yml
  format: yaml
  label: Postman API Versions API
  slug: postman-api-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-api-versions-api-openapi.yml
- filename: postman-mocks-api-openapi.yml
  format: yaml
  label: Postman Mocks API
  slug: postman-mocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-mocks-api-openapi.yml
- filename: postman-network-elements-api-openapi.yml
  format: yaml
  label: Postman Network Elements API
  slug: postman-network-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-network-elements-api-openapi.yml
- filename: postman-network-folders-api-openapi.yml
  format: yaml
  label: Postman Network Folders API
  slug: postman-network-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-network-folders-api-openapi.yml
- filename: postman-network-requests-api-openapi.yml
  format: yaml
  label: Postman Network Requests API
  slug: postman-network-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-network-requests-api-openapi.yml
- filename: postman-server-responses-api-openapi.yml
  format: yaml
  label: Postman Server Responses API
  slug: postman-server-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-server-responses-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Postman Authentication
name_suffix: Authentication
oauth_flows: []
overview: Postman secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Postman
provider_slug: postman
scheme_count: 1
schemes:
- description: Postman API key for authentication.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/postman-apis-api-openapi.yml
  - openapi/postman-audit-logs-api-openapi.yml
  - openapi/postman-collection-runs-api-openapi.yml
  - openapi/postman-collections-api-openapi.yml
  - openapi/postman-environments-api-openapi.yml
  - openapi/postman-mock-servers-api-openapi.yml
  - openapi/postman-monitors-api-openapi.yml
  - openapi/postman-private-api-network-api-openapi.yml
  - openapi/postman-secret-scanner-api-openapi.yml
  - openapi/postman-tags-api-openapi.yml
  - openapi/postman-webhooks-api-openapi.yml
  - openapi/postman-workspaces-api-openapi.yml
  type: apiKey
slug: postman-authentication
source_filename: postman-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/postman-apis-api-openapi.yml, openapi/postman-audit-logs-api-openapi.yml, openapi/postman-collection-runs-api-openapi.yml,\n  openapi/postman-collections-api-openapi.yml, openapi/postman-environments-api-openapi.yml,\n  openapi/postman-mock-servers-api-openapi.yml, openapi/postman-monitors-api-openapi.yml, openapi/postman-private-api-network-api-openapi.yml,\n  openapi/postman-secret-scanner-api-openapi.yml, openapi/postman-tags-api-openapi.yml, openapi/postman-webhooks-api-openapi.yml,\n  openapi/postman-workspaces-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Postman API key for authentication.\n  sources:\n  - openapi/postman-apis-api-openapi.yml\n  - openapi/postman-audit-logs-api-openapi.yml\n  - openapi/postman-collection-runs-api-openapi.yml\n  - openapi/postman-collections-api-openapi.yml\n\
  \  - openapi/postman-environments-api-openapi.yml\n  - openapi/postman-mock-servers-api-openapi.yml\n  - openapi/postman-monitors-api-openapi.yml\n  - openapi/postman-private-api-network-api-openapi.yml\n  - openapi/postman-secret-scanner-api-openapi.yml\n  - openapi/postman-tags-api-openapi.yml\n  - openapi/postman-webhooks-api-openapi.yml\n  - openapi/postman-workspaces-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/authentication/postman-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Agent Builder
- AI Agents
- API Catalog
- API Client
- API Design
- API Development
- API Documentation
- API Governance
- API Lifecycle
- API Monitoring
- API Network
- API Platform
- API Testing
- Audit Logs
- Automation
- CI/CD
- Collaboration
- Collections
- Compliance
- Discovery
- Environments
- Flows
- GraphQL
- gRPC
- HTTP
- Insights
- MCP
- MCP Generator
- Mock Servers
- Mocking
- Monitors
- Newman
- OpenAPI
- Platform
- Private API Network
- Public API Network
- Secret Scanning
- Spec Hub
- Specifications
- SSO
- Testing
- Vault
- WebSocket
- Workflows
- Workspaces
---
