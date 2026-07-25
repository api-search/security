---
api_key_in: []
api_specs:
- filename: datafiniti-authentication-api-openapi.yml
  format: yaml
  label: Datafiniti Authentication API
  slug: datafiniti-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafiniti/refs/heads/main/openapi/datafiniti-authentication-api-openapi.yml
- filename: datafiniti-businesses-api-openapi.yml
  format: yaml
  label: Datafiniti Businesses API
  slug: datafiniti-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafiniti/refs/heads/main/openapi/datafiniti-businesses-api-openapi.yml
- filename: datafiniti-people-api-openapi.yml
  format: yaml
  label: Datafiniti People API
  slug: datafiniti-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafiniti/refs/heads/main/openapi/datafiniti-people-api-openapi.yml
- filename: datafiniti-products-api-openapi.yml
  format: yaml
  label: Datafiniti Products API
  slug: datafiniti-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafiniti/refs/heads/main/openapi/datafiniti-products-api-openapi.yml
- filename: datafiniti-properties-api-openapi.yml
  format: yaml
  label: Datafiniti Properties API
  slug: datafiniti-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafiniti/refs/heads/main/openapi/datafiniti-properties-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Datafiniti Authentication
name_suffix: Authentication
oauth_flows: []
overview: Datafiniti secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Datafiniti
provider_slug: datafiniti
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/datafiniti-api.yml
  type: http
slug: datafiniti-authentication
source_filename: datafiniti-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datafiniti-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/datafiniti-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datafiniti/refs/heads/main/authentication/datafiniti-authentication.yml
summary_line: http · 1 scheme
tags:
- Business Data
- Data Aggregation
- Data as a Service
- People Data
- Product Data
- Property Data
---
