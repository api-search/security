---
anonymous_access: false
api_key_in: []
api_specs:
- filename: actian-access-tokens-api-openapi.yml
  format: yaml
  label: Actian Corporation Access Tokens API
  slug: actian-access-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-access-tokens-api-openapi.yml
- filename: actian-admin-user-api-openapi.yml
  format: yaml
  label: Actian Corporation Admin User API
  slug: actian-admin-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-admin-user-api-openapi.yml
- filename: actian-collections-api-openapi.yml
  format: yaml
  label: Actian Corporation Collections API
  slug: actian-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-collections-api-openapi.yml
- filename: actian-count-api-openapi.yml
  format: yaml
  label: Actian Corporation Count API
  slug: actian-count-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-count-api-openapi.yml
- filename: actian-filters-api-openapi.yml
  format: yaml
  label: Actian Corporation Filters API
  slug: actian-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-filters-api-openapi.yml
- filename: actian-points-api-openapi.yml
  format: yaml
  label: Actian Corporation Points API
  slug: actian-points-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-points-api-openapi.yml
- filename: actian-scroll-api-openapi.yml
  format: yaml
  label: Actian Corporation Scroll API
  slug: actian-scroll-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-scroll-api-openapi.yml
- filename: actian-search-api-openapi.yml
  format: yaml
  label: Actian Corporation Search API
  slug: actian-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-search-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Actian Authentication
name_suffix: Authentication
oauth_flows: []
overview: Actian Corporation secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Actian Corporation
provider_slug: actian
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Admin JWT obtained from the login endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/authentication-api.yaml
  - openapi/collections-api.yaml
  - openapi/filters-api.yaml
  - openapi/grouped-search-api.yaml
  - openapi/points-api.yaml
  - openapi/search-api.yaml
  type: http
slug: actian-authentication
source_filename: actian-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: derived\nsource: openapi/authentication-api.yaml, openapi/collections-api.yaml, openapi/filters-api.yaml,\n  openapi/grouped-search-api.yaml, openapi/points-api.yaml, openapi/search-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Admin JWT obtained from the login endpoint.\n  sources:\n  - openapi/authentication-api.yaml\n  - openapi/collections-api.yaml\n  - openapi/filters-api.yaml\n  - openapi/grouped-search-api.yaml\n  - openapi/points-api.yaml\n  - openapi/search-api.yaml\n"
source_yaml_url: https://artifacts.apis.io/actian/authentication/actian-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data
- Integration
- Analytics
- Artificial Intelligence
- Enterprise
---
