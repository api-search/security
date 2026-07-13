---
api_key_in: []
api_specs:
- filename: decodable-openapi.yml
  format: yaml
  label: Decodable Connections API
  slug: decodable-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/openapi/decodable-openapi.yml
- filename: decodable-openapi.yml
  format: yaml
  label: Decodable Streams API
  slug: decodable-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/openapi/decodable-openapi.yml
- filename: decodable-openapi.yml
  format: yaml
  label: Decodable Pipelines API
  slug: decodable-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/openapi/decodable-openapi.yml
- filename: decodable-openapi.yml
  format: yaml
  label: Decodable Secrets API
  slug: decodable-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/openapi/decodable-openapi.yml
- filename: decodable-openapi.yml
  format: yaml
  label: Decodable Resources API
  slug: decodable-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/openapi/decodable-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Decodable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Decodable secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Decodable
provider_slug: decodable
scheme_count: 1
schemes:
- description: 'Decodable access token issued after CLI login (stored in ~/.decodable/auth), sent as an Authorization: Bearer header.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/decodable-openapi.yml
  type: http
slug: decodable-authentication
source_filename: decodable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/decodable-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Decodable access token issued after CLI login (stored in ~/.decodable/auth),\n    sent as an Authorization: Bearer header.'\n  sources:\n  - openapi/decodable-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/authentication/decodable-authentication.yml
summary_line: http · 1 scheme
tags:
- Stream Processing
- Apache Flink
- Debezium
- Real Time Data
- Data Pipelines
- CDC
---
