---
api_key_in:
- header
api_specs:
- filename: edge-delta-access-api-openapi.yml
  format: yaml
  label: Edge Delta Access API
  slug: edge-delta-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-access-api-openapi.yml
- filename: edge-delta-add-source-api-openapi.yml
  format: yaml
  label: Edge Delta Add Source API
  slug: edge-delta-add-source-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-add-source-api-openapi.yml
- filename: edge-delta-agent-configs-api-openapi.yml
  format: yaml
  label: Edge Delta Agent Configs API
  slug: edge-delta-agent-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-agent-configs-api-openapi.yml
- filename: edge-delta-ai-api-openapi.yml
  format: yaml
  label: Edge Delta AI API
  slug: edge-delta-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-ai-api-openapi.yml
- filename: edge-delta-event-search-api-openapi.yml
  format: yaml
  label: Edge Delta Event Search API
  slug: edge-delta-event-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-event-search-api-openapi.yml
- filename: edge-delta-get-dashboard-api-openapi.yml
  format: yaml
  label: Edge Delta Get Dashboard API
  slug: edge-delta-get-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-get-dashboard-api-openapi.yml
- filename: edge-delta-get-dashboards-api-openapi.yml
  format: yaml
  label: Edge Delta Get Dashboards API
  slug: edge-delta-get-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-get-dashboards-api-openapi.yml
- filename: edge-delta-get-metrics-api-openapi.yml
  format: yaml
  label: Edge Delta Get Metrics API
  slug: edge-delta-get-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-get-metrics-api-openapi.yml
- filename: edge-delta-group-members-api-openapi.yml
  format: yaml
  label: Edge Delta Group Members API
  slug: edge-delta-group-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-group-members-api-openapi.yml
- filename: edge-delta-groups-api-openapi.yml
  format: yaml
  label: Edge Delta Groups API
  slug: edge-delta-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-groups-api-openapi.yml
- filename: edge-delta-integrations-api-openapi.yml
  format: yaml
  label: Edge Delta Integrations API
  slug: edge-delta-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-integrations-api-openapi.yml
- filename: edge-delta-log-search-api-openapi.yml
  format: yaml
  label: Edge Delta Log Search API
  slug: edge-delta-log-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-log-search-api-openapi.yml
- filename: edge-delta-lookup-tables-api-openapi.yml
  format: yaml
  label: Edge Delta Lookup Tables API
  slug: edge-delta-lookup-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-lookup-tables-api-openapi.yml
- filename: edge-delta-pattern-stats-api-openapi.yml
  format: yaml
  label: Edge Delta Pattern Stats API
  slug: edge-delta-pattern-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-pattern-stats-api-openapi.yml
- filename: edge-delta-pipeline-api-openapi.yml
  format: yaml
  label: Edge Delta Pipeline API
  slug: edge-delta-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-pipeline-api-openapi.yml
- filename: edge-delta-public-api-openapi.yml
  format: yaml
  label: Edge Delta Public API
  slug: edge-delta-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-public-api-openapi.yml
- filename: edge-delta-rehydrations-api-openapi.yml
  format: yaml
  label: Edge Delta Rehydrations API
  slug: edge-delta-rehydrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-rehydrations-api-openapi.yml
- filename: edge-delta-servedbymcp-api-openapi.yml
  format: yaml
  label: Edge Delta ServedByMCP API
  slug: edge-delta-servedbymcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-servedbymcp-api-openapi.yml
- filename: edge-delta-users-api-openapi.yml
  format: yaml
  label: Edge Delta Users API
  slug: edge-delta-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Edge Delta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Edge Delta secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Edge Delta
provider_slug: edge-delta
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-ED-API-Token
  sources:
  - openapi/edge-delta-openapi-original.json
  type: apiKey
slug: edge-delta-authentication
source_filename: edge-delta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/edge-delta-openapi-original.json\ndocs: https://docs.edgedelta.com/api-tokens/\nnotes: >-\n  Per-organization API token passed in the X-ED-API-Token header. Tokens are\n  created at https://docs.edgedelta.com/create-api-token/; the organization ID\n  (used in the {org_id} path scope) is obtained per https://docs.edgedelta.com/get-org-id/.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-ED-API-Token\n  sources:\n  - openapi/edge-delta-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/authentication/edge-delta-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Observability
- Telemetry Pipelines
- Logging
- Metrics
- Tracing
- Monitoring
- DevOps
- SRE
- Artificial Intelligence
---
