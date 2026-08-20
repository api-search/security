---
api_key_in: []
api_specs:
- filename: feldera-input-connectors-api-openapi.yml
  format: yaml
  label: Feldera Input Connectors API
  slug: feldera-input-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feldera/refs/heads/main/openapi/feldera-input-connectors-api-openapi.yml
- filename: feldera-metrics-debugging-api-openapi.yml
  format: yaml
  label: Feldera Metrics & Debugging API
  slug: feldera-metrics-debugging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feldera/refs/heads/main/openapi/feldera-metrics-debugging-api-openapi.yml
- filename: feldera-output-connectors-api-openapi.yml
  format: yaml
  label: Feldera Output Connectors API
  slug: feldera-output-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feldera/refs/heads/main/openapi/feldera-output-connectors-api-openapi.yml
- filename: feldera-pipeline-crud-api-openapi.yml
  format: yaml
  label: Feldera Pipeline CRUD API
  slug: feldera-pipeline-crud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feldera/refs/heads/main/openapi/feldera-pipeline-crud-api-openapi.yml
- filename: feldera-pipeline-lifecycle-api-openapi.yml
  format: yaml
  label: Feldera Pipeline Lifecycle API
  slug: feldera-pipeline-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feldera/refs/heads/main/openapi/feldera-pipeline-lifecycle-api-openapi.yml
- filename: feldera-platform-api-openapi.yml
  format: yaml
  label: Feldera Platform API
  slug: feldera-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feldera/refs/heads/main/openapi/feldera-platform-api-openapi.yml
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
- Data Pipeline
---
