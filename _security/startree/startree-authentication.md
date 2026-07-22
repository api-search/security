---
api_key_in: []
api_specs:
- filename: startree-query-openapi.json
  format: json
  label: StarTree Cloud Query API
  slug: startree-cloud-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/startree/refs/heads/main/openapi/startree-query-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Startree Authentication
name_suffix: Authentication
oauth_flows: []
overview: StarTree secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: StarTree
provider_slug: startree
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/startree-query-openapi.json
  type: http
slug: startree-authentication
source_filename: startree-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/startree-query-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/startree-query-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/startree/refs/heads/main/authentication/startree-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data
- Analytics
- Real-Time Analytics
- OLAP
- Apache Pinot
- Streaming
- Database
---
