---
anonymous_access: false
api_key_in: []
api_specs:
- filename: zh-ch-collector-configuration-api-openapi.yml
  format: yaml
  label: Kanton Zürich Collector configuration API
  slug: zh-ch-collector-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zh-ch/openapi/zh-ch-collector-configuration-api-openapi.yml
- filename: zh-ch-collector-state-api-openapi.yml
  format: yaml
  label: Kanton Zürich Collector state API
  slug: zh-ch-collector-state-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zh-ch/openapi/zh-ch-collector-state-api-openapi.yml
- filename: zh-ch-funktional-api-openapi.yml
  format: yaml
  label: Kanton Zürich Funktional API
  slug: zh-ch-funktional-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zh-ch/openapi/zh-ch-funktional-api-openapi.yml
- filename: zh-ch-online-data-api-openapi.yml
  format: yaml
  label: Kanton Zürich Online Data API
  slug: zh-ch-online-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zh-ch/openapi/zh-ch-online-data-api-openapi.yml
- filename: zh-ch-tests-api-openapi.yml
  format: yaml
  label: Kanton Zürich Tests API
  slug: zh-ch-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zh-ch/openapi/zh-ch-tests-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Kanton Zürich Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kanton Zürich secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kanton Zürich
provider_slug: zh-ch
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zh-ch-education-statistics-openapi.yml
  type: http
slug: zh-ch-authentication
source_filename: zh-ch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/zh-ch-education-statistics-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/zh-ch-education-statistics-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/zh-ch/authentication/zh-ch-authentication.yml
summary_line: http · 1 scheme
tags:
- Government
- Open Data
- Switzerland
- Statistics
- Traffic
- Education
- Geodata
---
