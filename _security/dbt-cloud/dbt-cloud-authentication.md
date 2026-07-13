---
api_key_in: []
api_specs:
- filename: dbt-cloud-openapi.yml
  format: yaml
  label: dbt Cloud Administrative API
  slug: dbt-cloud-administrative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-cloud/refs/heads/main/openapi/dbt-cloud-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dbt Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: dbt Cloud secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: dbt Cloud
provider_slug: dbt-cloud
scheme_count: 1
schemes:
- description: 'dbt Cloud service token or personal access token passed in the Authorization header as ''Authorization: Token <token>'' or ''Authorization: Bearer <token>''.'
  name: BearerAuthentication
  scheme: bearer
  sources:
  - openapi/dbt-cloud-openapi.yml
  type: http
slug: dbt-cloud-authentication
source_filename: dbt-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dbt-cloud-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuthentication\n  type: http\n  scheme: bearer\n  description: 'dbt Cloud service token or personal access token passed in the Authorization\n    header as ''Authorization: Token <token>'' or ''Authorization: Bearer <token>''.'\n  sources:\n  - openapi/dbt-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dbt-cloud/refs/heads/main/authentication/dbt-cloud-authentication.yml
summary_line: http · 1 scheme
tags:
- Data
- Analytics Engineering
- Data Transformation
- ELT
- Semantic Layer
---
