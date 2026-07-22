---
api_key_in: []
api_specs:
- filename: startree-cortexdata-query-openapi.json
  format: json
  label: StarTree Cloud Query API
  slug: startree-cloud-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/startree-cortexdata/refs/heads/main/openapi/startree-cortexdata-query-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Startree Cortexdata Authentication
name_suffix: Authentication
oauth_flows: []
overview: StarTree (Cortexdata) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: StarTree (Cortexdata)
provider_slug: startree-cortexdata
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/startree-cortexdata-query-openapi.json
  type: http
slug: startree-cortexdata-authentication
source_filename: startree-cortexdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/startree-cortexdata-query-openapi.json\ndocs: https://docs.startree.ai/api-reference/introduction\nnotes: >-\n  StarTree Cloud authenticates with a Bearer token (JWT) generated in the\n  console under API Access. The token must be included on every request. A\n  `database` HTTP header carries the Workspace ID (e.g. ws_2kc8e2dnzzb0) for\n  multi-tenant (Free Tier) clusters; it is not required for dedicated clusters.\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/startree-cortexdata-query-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/startree-cortexdata/refs/heads/main/authentication/startree-cortexdata-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai Infrastructure
- Real-Time Analytics
- Apache Pinot
- OLAP
- Analytics
- Streaming Data
- Database
---
