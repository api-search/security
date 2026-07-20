---
api_key_in: []
api_specs:
- filename: feldera-openapi-original.json
  format: json
  label: Feldera API
  slug: feldera-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feldera/refs/heads/main/openapi/feldera-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Feldera Authentication
name_suffix: Authentication
oauth_flows: []
overview: Feldera secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Feldera
provider_slug: feldera
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: "Use a JWT token obtained via an OAuth2/OIDC\n                               login workflow or an API key obtained via\n                               the `/v0/api-keys` endpoint."
  name: JSON web token (JWT) or API key
  scheme: bearer
  sources:
  - openapi/feldera-openapi-original.json
  type: http
slug: feldera-authentication
source_filename: feldera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/feldera-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: JSON web token (JWT) or API key\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Use a JWT token obtained via an OAuth2/OIDC\n                                   login workflow or an API key obtained via\n                                   the `/v0/api-keys` endpoint.\n  sources:\n  - openapi/feldera-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/feldera/refs/heads/main/authentication/feldera-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data Infrastructure
- Streaming
- SQL
- Incremental View Maintenance
- Real-Time Analytics
- Change Data Capture
- Materialized Views
- Data Pipelines
---
