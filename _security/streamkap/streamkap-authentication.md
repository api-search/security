---
api_key_in: []
api_specs:
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Sources API
  slug: streamkap-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Destinations API
  slug: streamkap-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Pipelines API
  slug: streamkap-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Connectors API
  slug: streamkap-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Transforms API
  slug: streamkap-transforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Topics API
  slug: streamkap-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Tags API
  slug: streamkap-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Kafka Access API
  slug: streamkap-kafka-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Authentication API
  slug: streamkap-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Streamkap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Streamkap secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Streamkap
provider_slug: streamkap
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'JWT access token obtained from POST /authentication/access-token by exchanging a client-id and secret (or a project key). Passed as Authorization: Bearer <token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/streamkap-openapi.yml
  type: http
slug: streamkap-authentication
source_filename: streamkap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/streamkap-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT access token obtained from POST /authentication/access-token by exchanging\n    a client-id and secret (or a project key). Passed as Authorization: Bearer <token>.'\n  sources:\n  - openapi/streamkap-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/authentication/streamkap-authentication.yml
summary_line: http · 1 scheme
tags:
- Streaming
- ETL
- CDC
- Kafka
- Flink
- Data Integration
- Real Time
---
