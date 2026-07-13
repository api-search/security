---
api_key_in: []
api_specs:
- filename: sentera-openapi.yml
  format: yaml
  label: Sentera FieldAgent GraphQL API
  slug: sentera-fieldagent-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentera/refs/heads/main/openapi/sentera-openapi.yml
- filename: sentera-openapi.yml
  format: yaml
  label: Sentera Imagery & Data API
  slug: sentera-imagery-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentera/refs/heads/main/openapi/sentera-openapi.yml
- filename: sentera-openapi.yml
  format: yaml
  label: Sentera Plot Analytics API
  slug: sentera-plot-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentera/refs/heads/main/openapi/sentera-openapi.yml
- filename: sentera-openapi.yml
  format: yaml
  label: Sentera Orders & Organizations API
  slug: sentera-orders-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentera/refs/heads/main/openapi/sentera-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sentera Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sentera secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sentera
provider_slug: sentera
scheme_count: 1
schemes:
- description: 'Sentera auth_token presented as `Authorization: Bearer <auth_token>`. See the Authentication and Authorization documentation for obtaining a token.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sentera-openapi.yml
  type: http
slug: sentera-authentication
source_filename: sentera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sentera-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Sentera auth_token presented as `Authorization: Bearer <auth_token>`. See the\n    Authentication and Authorization documentation for obtaining a token.'\n  sources:\n  - openapi/sentera-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentera/refs/heads/main/authentication/sentera-authentication.yml
summary_line: http · 1 scheme
tags:
- Precision Agriculture
- Aerial Imagery
- Drones
- Sensors
- Analytics
- GraphQL
---
