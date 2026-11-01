---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dune-analytics-execution-api-openapi.yml
  format: yaml
  label: Dune Analytics Execution API
  slug: dune-analytics-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-execution-api-openapi.yml
- filename: dune-analytics-query-api-openapi.yml
  format: yaml
  label: Dune Analytics Query API
  slug: dune-analytics-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-query-api-openapi.yml
- filename: dune-analytics-contracts-api-openapi.yml
  format: yaml
  label: Dune Analytics Contracts API
  slug: dune-analytics-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-contracts-api-openapi.yml
- filename: dune-analytics-dashboards-api-openapi.yml
  format: yaml
  label: Dune Analytics Dashboards API
  slug: dune-analytics-dashboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-dashboards-api-openapi.yml
- filename: dune-analytics-datasets-api-openapi.yml
  format: yaml
  label: Dune Analytics Datasets API
  slug: dune-analytics-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-datasets-api-openapi.yml
- filename: dune-analytics-endpoints-api-openapi.yml
  format: yaml
  label: Dune Analytics Endpoints API
  slug: dune-analytics-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-endpoints-api-openapi.yml
- filename: dune-analytics-materialized-views-api-openapi.yml
  format: yaml
  label: Dune Analytics Materialized Views API
  slug: dune-analytics-materialized-views-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-materialized-views-api-openapi.yml
- filename: dune-analytics-pipelines-api-openapi.yml
  format: yaml
  label: Dune Analytics Pipelines API
  slug: dune-analytics-pipelines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-pipelines-api-openapi.yml
- filename: dune-analytics-queries-api-openapi.yml
  format: yaml
  label: Dune Analytics Queries API
  slug: dune-analytics-queries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-queries-api-openapi.yml
- filename: dune-analytics-sql-api-openapi.yml
  format: yaml
  label: Dune Analytics Sql API
  slug: dune-analytics-sql-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-sql-api-openapi.yml
- filename: dune-analytics-uploads-api-openapi.yml
  format: yaml
  label: Dune Analytics Uploads API
  slug: dune-analytics-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-uploads-api-openapi.yml
- filename: dune-analytics-usage-api-openapi.yml
  format: yaml
  label: Dune Analytics Usage API
  slug: dune-analytics-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-usage-api-openapi.yml
- filename: dune-analytics-visualizations-api-openapi.yml
  format: yaml
  label: Dune Analytics Visualizations API
  slug: dune-analytics-visualizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-visualizations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Dune Analytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dune Analytics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dune Analytics
provider_slug: dune-analytics
scheme_count: 1
schemes:
- in: header
  name: DuneApiKey
  parameter: X-Dune-API-Key
  sources:
  - openapi/dune-analytics-openapi.yml
  type: apiKey
slug: dune-analytics-authentication
source_filename: dune-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dune-analytics-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: DuneApiKey\n  type: apiKey\n  in: header\n  parameter: X-Dune-API-Key\n  sources:\n  - openapi/dune-analytics-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/dune-analytics/authentication/dune-analytics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Analytics
- SQL
- Dashboards
- Blockchain
- Onchain
- Multi-Chain
- Ethereum
---
