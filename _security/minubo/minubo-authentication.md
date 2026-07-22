---
api_key_in: []
api_specs:
- filename: minubo-api-openapi-original.json
  format: json
  label: Minubo API
  slug: minubo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/minubo/refs/heads/main/openapi/minubo-api-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Minubo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Minubo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Minubo
provider_slug: minubo
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT Authorization header using the Bearer scheme. Can be retrieved by authenticating with the /auth/v1/token endpoint.
  name: etl_bearerAuth
  scheme: bearer
  sources:
  - openapi/minubo-api-openapi-original.json
  type: http
slug: minubo-authentication
source_filename: minubo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/minubo-api-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: etl_bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT Authorization header using the Bearer scheme. Can be retrieved by authenticating\n    with the /auth/v1/token endpoint.\n  sources:\n  - openapi/minubo-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/minubo/refs/heads/main/authentication/minubo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- E-Commerce
- Business Intelligence
- Analytics
- Retail
- Data
- ETL
- Reporting
---
