---
anonymous_access: false
api_key_in: []
api_specs:
- filename: popsql-data-catalog-api-openapi.yml
  format: yaml
  label: PopSQL Data Catalog API
  slug: popsql-data-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/popsql/openapi/popsql-data-catalog-api-openapi.yml
- filename: popsql-query-runs-api-openapi.yml
  format: yaml
  label: PopSQL Query Runs API
  slug: popsql-query-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/popsql/openapi/popsql-query-runs-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Popsql Authentication
name_suffix: Authentication
oauth_flows: []
overview: PopSQL secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PopSQL
provider_slug: popsql
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/popsql-api-openapi.yml
  type: http
slug: popsql-authentication
source_filename: popsql-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/popsql-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/popsql-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/popsql/authentication/popsql-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- SQL
- Collaboration
- Data-Analytics
- Cloud
---
