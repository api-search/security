---
api_key_in:
- header
api_specs:
- filename: wundergraph-analytics-api-openapi.yml
  format: yaml
  label: WunderGraph Analytics API
  slug: wundergraph-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-analytics-api-openapi.yml
- filename: wundergraph-api-keys-api-openapi.yml
  format: yaml
  label: WunderGraph API Keys API
  slug: wundergraph-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-api-keys-api-openapi.yml
- filename: wundergraph-feature-flags-api-openapi.yml
  format: yaml
  label: WunderGraph Feature Flags API
  slug: wundergraph-feature-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-feature-flags-api-openapi.yml
- filename: wundergraph-feature-subgraphs-api-openapi.yml
  format: yaml
  label: WunderGraph Feature Subgraphs API
  slug: wundergraph-feature-subgraphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-feature-subgraphs-api-openapi.yml
- filename: wundergraph-federated-graphs-api-openapi.yml
  format: yaml
  label: WunderGraph Federated Graphs API
  slug: wundergraph-federated-graphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-federated-graphs-api-openapi.yml
- filename: wundergraph-monographs-api-openapi.yml
  format: yaml
  label: WunderGraph Monographs API
  slug: wundergraph-monographs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-monographs-api-openapi.yml
- filename: wundergraph-namespaces-api-openapi.yml
  format: yaml
  label: WunderGraph Namespaces API
  slug: wundergraph-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-namespaces-api-openapi.yml
- filename: wundergraph-router-api-openapi.yml
  format: yaml
  label: WunderGraph Router API
  slug: wundergraph-router-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-router-api-openapi.yml
- filename: wundergraph-schema-contracts-api-openapi.yml
  format: yaml
  label: WunderGraph Schema Contracts API
  slug: wundergraph-schema-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-schema-contracts-api-openapi.yml
- filename: wundergraph-subgraphs-api-openapi.yml
  format: yaml
  label: WunderGraph Subgraphs API
  slug: wundergraph-subgraphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-subgraphs-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wundergraph Authentication
name_suffix: Authentication
oauth_flows: []
overview: WunderGraph secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WunderGraph
provider_slug: wundergraph
scheme_count: 1
schemes:
- description: API key for authenticating with the Cosmo Platform API. Obtain via Cosmo Studio or wgc CLI. Set as COSMO_API_KEY environment variable.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/wundergraph-cosmo-platform-openapi.yml
  type: apiKey
slug: wundergraph-authentication
source_filename: wundergraph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wundergraph-cosmo-platform-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key for authenticating with the Cosmo Platform API. Obtain via Cosmo Studio\n    or wgc CLI. Set as COSMO_API_KEY environment variable.\n  sources:\n  - openapi/wundergraph-cosmo-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/authentication/wundergraph-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Federation
- GraphQL
- Management
- Schema Registry
- API Gateway
- Observability
- Agents
- Developer Tools
---
