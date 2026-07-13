---
api_key_in: []
api_specs:
- filename: dbt-cloud-administrative-api-openapi.yml
  format: yaml
  label: dbt Cloud Administrative API
  slug: dbt-cloud-administrative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt/refs/heads/main/openapi/dbt-cloud-administrative-api-openapi.yml
- filename: dbt-cloud-discovery-api-openapi.yml
  format: yaml
  label: dbt Cloud Discovery API
  slug: dbt-cloud-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt/refs/heads/main/openapi/dbt-cloud-discovery-api-openapi.yml
- filename: dbt-cloud-semantic-layer-api-openapi.yml
  format: yaml
  label: dbt Cloud Semantic Layer API
  slug: dbt-cloud-semantic-layer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt/refs/heads/main/openapi/dbt-cloud-semantic-layer-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dbt/refs/heads/main/authentication/dbt-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics Engineering
- Data
- ELT
- Metrics
- Projects
- SQL
- Transformation
---
