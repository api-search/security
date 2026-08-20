---
api_key_in:
- header
api_specs:
- filename: agnost-ai-alerts-api-openapi.yml
  format: yaml
  label: Agnost AI Alerts API
  slug: agnost-ai-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/openapi/agnost-ai-alerts-api-openapi.yml
- filename: agnost-ai-api-keys-api-openapi.yml
  format: yaml
  label: Agnost AI API Keys API
  slug: agnost-ai-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/openapi/agnost-ai-api-keys-api-openapi.yml
- filename: agnost-ai-auth-api-openapi.yml
  format: yaml
  label: Agnost AI Auth API
  slug: agnost-ai-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/openapi/agnost-ai-auth-api-openapi.yml
- filename: agnost-ai-billing-api-openapi.yml
  format: yaml
  label: Agnost AI Billing API
  slug: agnost-ai-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/openapi/agnost-ai-billing-api-openapi.yml
- filename: agnost-ai-classification-api-openapi.yml
  format: yaml
  label: Agnost AI Classification API
  slug: agnost-ai-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/openapi/agnost-ai-classification-api-openapi.yml
- filename: agnost-ai-connections-api-openapi.yml
  format: yaml
  label: Agnost AI Connections API
  slug: agnost-ai-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/openapi/agnost-ai-connections-api-openapi.yml
- filename: agnost-ai-conversations-api-openapi.yml
  format: yaml
  label: Agnost AI Conversations API
  slug: agnost-ai-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/openapi/agnost-ai-conversations-api-openapi.yml
- filename: agnost-ai-dashboard-api-openapi.yml
  format: yaml
  label: Agnost AI Dashboard API
  slug: agnost-ai-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/openapi/agnost-ai-dashboard-api-openapi.yml
- filename: agnost-ai-onboarding-api-openapi.yml
  format: yaml
  label: Agnost AI Onboarding API
  slug: agnost-ai-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/openapi/agnost-ai-onboarding-api-openapi.yml
- filename: agnost-ai-organizations-api-openapi.yml
  format: yaml
  label: Agnost AI Organizations API
  slug: agnost-ai-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/openapi/agnost-ai-organizations-api-openapi.yml
- filename: agnost-ai-sdk-api-openapi.yml
  format: yaml
  label: Agnost AI SDK API
  slug: agnost-ai-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/openapi/agnost-ai-sdk-api-openapi.yml
- filename: agnost-ai-sentiments-api-openapi.yml
  format: yaml
  label: Agnost AI Sentiments API
  slug: agnost-ai-sentiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/openapi/agnost-ai-sentiments-api-openapi.yml
- filename: agnost-ai-sops-api-openapi.yml
  format: yaml
  label: Agnost AI SOPs API
  slug: agnost-ai-sops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/openapi/agnost-ai-sops-api-openapi.yml
- filename: agnost-ai-system-api-openapi.yml
  format: yaml
  label: Agnost AI System API
  slug: agnost-ai-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/openapi/agnost-ai-system-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Agnost Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agnost AI secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Agnost AI
provider_slug: agnost-ai
scheme_count: 3
schemes:
- description: Organization ID (UUID). Used by SDKs for event ingestion. Header is case-insensitive.
  in: header
  name: OrgId
  parameter: x-org-id
  sources:
  - openapi/agnost-ai-openapi-original.yml
  type: apiKey
- bearerFormat: JWT
  description: JWT token from OAuth login.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/agnost-ai-openapi-original.yml
  type: http
- description: API key (`agnost_<64-hex>`) for programmatic dashboard access. Issued via Settings → API Keys.
  in: header
  name: ApiKey
  parameter: x-api-key
  sources:
  - openapi/agnost-ai-openapi-original.yml
  type: apiKey
slug: agnost-ai-authentication
source_filename: agnost-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/agnost-ai-openapi-original.yml\ndocs: https://docs.agnost.ai/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  models:\n  - name: SDK ingestion\n    endpoints: /api/v1/*\n    credential: x-org-id header (organization UUID; public routing identifier, not a secret)\n  - name: Dashboard/API (JWT)\n    credential: 'Authorization: Bearer <jwt> + x-org-id'\n    use: browser/dashboard access after Google OAuth login\n  - name: Dashboard/API (API key)\n    credential: x-api-key (agnost_<64-hex>) + optional x-org-id\n    use: programmatic dashboard/API access; issued from Settings -> API Keys\n  - name: OpenTelemetry ingestion\n    endpoint: https://otel.agnost.ai/v1/traces\n    credential: 'OTEL_EXPORTER_OTLP_HEADERS=X-Agnost-Org-ID=<org-id>'\n  - name: MCP server\n    endpoint: https://mcp.agnost.ai/mcp\n    credential: OAuth 2.1 (dynamic client registration, Google identity)\nschemes:\n\
  - name: OrgId\n  type: apiKey\n  in: header\n  parameter: x-org-id\n  description: Organization ID (UUID). Used by SDKs for event ingestion. Header is case-insensitive.\n  sources:\n  - openapi/agnost-ai-openapi-original.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token from OAuth login.\n  sources:\n  - openapi/agnost-ai-openapi-original.yml\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key (`agnost_<64-hex>`) for programmatic dashboard access. Issued via Settings\n    → API Keys.\n  sources:\n  - openapi/agnost-ai-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/authentication/agnost-ai-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- AI Agents
- Agent Analytics
- Observability
- OpenTelemetry
- MCP
- Conversational AI
- Monitoring
- Developer Tools
- Analytics
---
