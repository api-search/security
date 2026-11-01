---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dbt-accounts-api-openapi.yml
  format: yaml
  label: dbt Accounts API
  slug: dbt-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-accounts-api-openapi.yml
- filename: dbt-environments-api-openapi.yml
  format: yaml
  label: dbt Environments API
  slug: dbt-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-environments-api-openapi.yml
- filename: dbt-jobs-api-openapi.yml
  format: yaml
  label: dbt Jobs API
  slug: dbt-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-jobs-api-openapi.yml
- filename: dbt-metrics-api-openapi.yml
  format: yaml
  label: dbt Metrics API
  slug: dbt-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-metrics-api-openapi.yml
- filename: dbt-projects-api-openapi.yml
  format: yaml
  label: dbt Projects API
  slug: dbt-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-projects-api-openapi.yml
- filename: dbt-runs-api-openapi.yml
  format: yaml
  label: dbt Runs API
  slug: dbt-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-runs-api-openapi.yml
- filename: dbt-fastapi-api-openapi.yml
  format: yaml
  label: dbt Fast API
  slug: dbt-fastapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-fastapi-api-openapi.yml
- filename: dbt-private-api-openapi.yml
  format: yaml
  label: dbt Private API
  slug: dbt-private-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-private-api-openapi.yml
- filename: dbt-ready-api-openapi.yml
  format: yaml
  label: dbt Ready API
  slug: dbt-ready-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-ready-api-openapi.yml
- filename: dbt-graph-ql-api-openapi.yml
  format: yaml
  label: dbt Graph QL API
  slug: dbt-graph-ql-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-graph-ql-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Dbt Authentication
name_suffix: Authentication
oauth_flows: []
overview: dbt secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: dbt
provider_slug: dbt
scheme_count: 1
schemes:
- bearerFormat: Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dbt-cloud-administrative-api-openapi.yml
  - openapi/dbt-cloud-discovery-api-openapi.yml
  - openapi/dbt-cloud-semantic-layer-api-openapi.yml
  type: http
slug: dbt-authentication
source_filename: dbt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dbt-cloud-administrative-api-openapi.yml, openapi/dbt-cloud-discovery-api-openapi.yml,\n  openapi/dbt-cloud-semantic-layer-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Token\n  sources:\n  - openapi/dbt-cloud-administrative-api-openapi.yml\n  - openapi/dbt-cloud-discovery-api-openapi.yml\n  - openapi/dbt-cloud-semantic-layer-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/dbt/authentication/dbt-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics Engineering
- Data
- ELT
- Metrics
- Project
- SQL
- Transformation
---
