---
anonymous_access: false
api_key_in: []
api_specs:
- filename: praisecharts-catalog-api-openapi.yml
  format: yaml
  label: PraiseCharts Catalog API
  slug: praisecharts-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/praisecharts/openapi/praisecharts-catalog-api-openapi.yml
- filename: praisecharts-download-api-openapi.yml
  format: yaml
  label: PraiseCharts Download API
  slug: praisecharts-download-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/praisecharts/openapi/praisecharts-download-api-openapi.yml
- filename: praisecharts-library-api-openapi.yml
  format: yaml
  label: PraiseCharts Library API
  slug: praisecharts-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/praisecharts/openapi/praisecharts-library-api-openapi.yml
- filename: praisecharts-oauth-api-openapi.yml
  format: yaml
  label: PraiseCharts OAuth API
  slug: praisecharts-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/praisecharts/openapi/praisecharts-oauth-api-openapi.yml
- filename: praisecharts-user-api-openapi.yml
  format: yaml
  label: PraiseCharts User API
  slug: praisecharts-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/praisecharts/openapi/praisecharts-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: PraiseCharts Authentication
name_suffix: Authentication
oauth_flows: []
overview: PraiseCharts secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PraiseCharts
provider_slug: praisecharts
scheme_count: 1
schemes:
- description: OAuth 1.0a
  name: Authorization
  scheme: oauth
  sources:
  - openapi/praisecharts-openapi.json
  type: http
slug: praisecharts-authentication
source_filename: praisecharts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/praisecharts-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Authorization\n  type: http\n  scheme: oauth\n  description: OAuth 1.0a\n  sources:\n  - openapi/praisecharts-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/praisecharts/authentication/praisecharts-authentication.yml
summary_line: http · 1 scheme
tags:
- Music
- Christian
- Worship
- Sheet Music
- E-Commerce
---
