---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datagraph-city-admin-api-openapi.yml
  format: yaml
  label: DataGraph.city Admin API
  slug: datagraph-city-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-admin-api-openapi.yml
- filename: datagraph-city-analytics-api-openapi.yml
  format: yaml
  label: DataGraph.city Analytics API
  slug: datagraph-city-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-analytics-api-openapi.yml
- filename: datagraph-city-api-key-api-openapi.yml
  format: yaml
  label: DataGraph.city Api Key API
  slug: datagraph-city-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-api-key-api-openapi.yml
- filename: datagraph-city-authorize-api-openapi.yml
  format: yaml
  label: DataGraph.city Authorize API
  slug: datagraph-city-authorize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-authorize-api-openapi.yml
- filename: datagraph-city-billing-api-openapi.yml
  format: yaml
  label: DataGraph.city Billing API
  slug: datagraph-city-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-billing-api-openapi.yml
- filename: datagraph-city-cities-api-openapi.yml
  format: yaml
  label: DataGraph.city Cities API
  slug: datagraph-city-cities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-cities-api-openapi.yml
- filename: datagraph-city-datasets-api-openapi.yml
  format: yaml
  label: DataGraph.city Datasets API
  slug: datagraph-city-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-datasets-api-openapi.yml
- filename: datagraph-city-health-api-openapi.yml
  format: yaml
  label: DataGraph.city Health API
  slug: datagraph-city-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-health-api-openapi.yml
- filename: datagraph-city-mcp-api-openapi.yml
  format: yaml
  label: DataGraph.city MCP API
  slug: datagraph-city-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-mcp-api-openapi.yml
- filename: datagraph-city-me-api-openapi.yml
  format: yaml
  label: DataGraph.city Me API
  slug: datagraph-city-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-me-api-openapi.yml
- filename: datagraph-city-metrics-api-openapi.yml
  format: yaml
  label: DataGraph.city Metrics API
  slug: datagraph-city-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-metrics-api-openapi.yml
- filename: datagraph-city-query-api-openapi.yml
  format: yaml
  label: DataGraph.city Query API
  slug: datagraph-city-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-query-api-openapi.yml
- filename: datagraph-city-resend-api-key-api-openapi.yml
  format: yaml
  label: DataGraph.city Resend Api Key API
  slug: datagraph-city-resend-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-resend-api-key-api-openapi.yml
- filename: datagraph-city-schema-api-openapi.yml
  format: yaml
  label: DataGraph.city Schema API
  slug: datagraph-city-schema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-schema-api-openapi.yml
- filename: datagraph-city-signup-api-openapi.yml
  format: yaml
  label: DataGraph.city Signup API
  slug: datagraph-city-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-signup-api-openapi.yml
- filename: datagraph-city-token-api-openapi.yml
  format: yaml
  label: DataGraph.city Token API
  slug: datagraph-city-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-token-api-openapi.yml
- filename: datagraph-city-usage-api-openapi.yml
  format: yaml
  label: DataGraph.city Usage API
  slug: datagraph-city-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-usage-api-openapi.yml
- filename: datagraph-city-webhooks-api-openapi.yml
  format: yaml
  label: DataGraph.city Webhooks API
  slug: datagraph-city-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-webhooks-api-openapi.yml
- filename: datagraph-city-well-known-api-openapi.yml
  format: yaml
  label: DataGraph.city .well Known API
  slug: datagraph-city-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-well-known-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: DataGraph.city Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataGraph.city secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DataGraph.city
provider_slug: datagraph-city
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/datagraph-city-openapi.json
  type: http
slug: datagraph-city-authentication
source_filename: datagraph-city-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/datagraph-city-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/datagraph-city-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/datagraph-city/authentication/datagraph-city-authentication.yml
summary_line: http · 1 scheme
tags:
- Urban Data
- Artificial Intelligence
- MCP
- Graph RAG
- PrivateBeta
---
