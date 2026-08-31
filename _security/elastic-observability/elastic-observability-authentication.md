---
api_key_in:
- header
api_specs:
- filename: elastic-observability-server-info-api-openapi.yml
  format: yaml
  label: Elastic Observability Server Info API
  slug: elastic-observability-server-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-observability/refs/heads/main/openapi/elastic-observability-server-info-api-openapi.yml
- filename: elastic-observability-agent-config-api-openapi.yml
  format: yaml
  label: Elastic Observability agent config API
  slug: elastic-observability-agent-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-observability/refs/heads/main/openapi/elastic-observability-agent-config-api-openapi.yml
- filename: elastic-observability-event-intake-api-openapi.yml
  format: yaml
  label: Elastic Observability event intake API
  slug: elastic-observability-event-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-observability/refs/heads/main/openapi/elastic-observability-event-intake-api-openapi.yml
- filename: elastic-observability-opentelemetry-intake-api-openapi.yml
  format: yaml
  label: Elastic Observability opentelemetry intake API
  slug: elastic-observability-opentelemetry-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-observability/refs/heads/main/openapi/elastic-observability-opentelemetry-intake-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Elastic Observability Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elastic Observability secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Elastic Observability
provider_slug: elastic-observability
scheme_count: 2
schemes:
- description: 'e.g. Authorization: ApiKey base64AccessApiKey'
  docs: https://www.elastic.co/docs/deploy-manage/api-keys
  header_format: 'Authorization: ApiKey <base64(id:api_key)>'
  in: header
  issued_by: Kibana / Elasticsearch security API — created per deployment, scoped by privileges
  name: apiKeyAuth
  parameter: Authorization
  revocable: true
  sources:
  - openapi/elastic-observability-agent-config-api-openapi.yml
  - openapi/elastic-observability-event-intake-api-openapi.yml
  - openapi/elastic-observability-opentelemetry-intake-api-openapi.yml
  - openapi/elastic-observability-server-info-api-openapi.yml
  type: apiKey
- bearerFormat: Secret token
  docs: https://www.elastic.co/docs/solutions/observability/apm/secret-token
  header_format: 'Authorization: Bearer <secret-token>'
  issued_by: Provisioned automatically when an Elastic Cloud Hosted or Elastic Cloud Enterprise deployment is created; found and reset in the Cloud console under the deployment's APM & Fleet page.
  name: secretToken
  note: Both the agent and the APM Server must be configured with the same secret token. Because it is shared and unscoped, an API key is the stronger choice where per-agent revocation matters.
  scheme: bearer
  scope: one shared token per APM Server — it authorizes agents, it does not identify them
  sources:
  - openapi/elastic-observability-agent-config-api-openapi.yml
  - openapi/elastic-observability-event-intake-api-openapi.yml
  - openapi/elastic-observability-opentelemetry-intake-api-openapi.yml
  - openapi/elastic-observability-server-info-api-openapi.yml
  type: http
slug: elastic-observability-authentication
source_filename: elastic-observability-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: 'openapi/elastic-observability-*-openapi.yml (schemes) enriched from Elastic''s own APM authentication\n  docs listed under docs:'\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'e.g. Authorization: ApiKey base64AccessApiKey'\n  sources:\n  - openapi/elastic-observability-agent-config-api-openapi.yml\n  - openapi/elastic-observability-event-intake-api-openapi.yml\n  - openapi/elastic-observability-opentelemetry-intake-api-openapi.yml\n  - openapi/elastic-observability-server-info-api-openapi.yml\n  header_format: 'Authorization: ApiKey <base64(id:api_key)>'\n  issued_by: Kibana / Elasticsearch security API — created per deployment, scoped by privileges\n  docs: https://www.elastic.co/docs/deploy-manage/api-keys\n  revocable: true\n- name: secretToken\n  type: http\n  scheme: bearer\n  bearerFormat: Secret\
  \ token\n  sources:\n  - openapi/elastic-observability-agent-config-api-openapi.yml\n  - openapi/elastic-observability-event-intake-api-openapi.yml\n  - openapi/elastic-observability-opentelemetry-intake-api-openapi.yml\n  - openapi/elastic-observability-server-info-api-openapi.yml\n  header_format: 'Authorization: Bearer <secret-token>'\n  issued_by: Provisioned automatically when an Elastic Cloud Hosted or Elastic Cloud Enterprise deployment\n    is created; found and reset in the Cloud console under the deployment's APM & Fleet page.\n  docs: https://www.elastic.co/docs/solutions/observability/apm/secret-token\n  scope: one shared token per APM Server — it authorizes agents, it does not identify them\n  note: Both the agent and the APM Server must be configured with the same secret token. Because it\n    is shared and unscoped, an API key is the stronger choice where per-agent revocation matters.\ndocs:\n- https://www.elastic.co/docs/solutions/observability/apm/secret-token\n- https://www.elastic.co/docs/solutions/observability/apm/api-keys\n\
  - https://www.elastic.co/docs/deploy-manage/api-keys\nnote: 'The two schemes are ALTERNATIVES, not a chain — the contract lists them as separate top-level\n  security requirements, so an agent sends one Authorization header, never both. Neither is OAuth: the\n  intake API declares no oauth2 securityScheme and no scopes exist to derive, which is why scopes/ is\n  absent from this repo rather than empty.'\nadjacent_surfaces:\n- surface: Elastic Agent Builder MCP server\n  methods:\n  - API key\n  - OAuth 2.1 authentication using an application connection\n  docs: https://www.elastic.co/docs/explore-analyze/ai-features/agent-builder/mcp-server\n  note: The only place Elastic documents OAuth for an Observability-adjacent surface. It is NOT part\n    of the intake contract above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elastic-observability/refs/heads/main/authentication/elastic-observability-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AIOps
- Observability
- APM
- Logging
- Metrics
- Tracing
- OpenTelemetry
- Monitoring
- Telemetry
---
