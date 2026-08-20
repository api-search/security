---
api_key_in:
- header
api_specs:
- filename: qdrant-aliases-api-openapi.yml
  format: yaml
  label: Qdrant Aliases API
  slug: qdrant-aliases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-aliases-api-openapi.yml
- filename: qdrant-beta-api-openapi.yml
  format: yaml
  label: Qdrant Beta API
  slug: qdrant-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-beta-api-openapi.yml
- filename: qdrant-collections-api-openapi.yml
  format: yaml
  label: Qdrant Collections API
  slug: qdrant-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-collections-api-openapi.yml
- filename: qdrant-distributed-api-openapi.yml
  format: yaml
  label: Qdrant Distributed API
  slug: qdrant-distributed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-distributed-api-openapi.yml
- filename: qdrant-indexes-api-openapi.yml
  format: yaml
  label: Qdrant Indexes API
  slug: qdrant-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-indexes-api-openapi.yml
- filename: qdrant-points-api-openapi.yml
  format: yaml
  label: Qdrant Points API
  slug: qdrant-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-points-api-openapi.yml
- filename: qdrant-search-api-openapi.yml
  format: yaml
  label: Qdrant Search API
  slug: qdrant-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-search-api-openapi.yml
- filename: qdrant-service-api-openapi.yml
  format: yaml
  label: Qdrant Service API
  slug: qdrant-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-service-api-openapi.yml
- filename: qdrant-snapshots-api-openapi.yml
  format: yaml
  label: Qdrant Snapshots API
  slug: qdrant-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-snapshots-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Qdrant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qdrant secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Qdrant
provider_slug: qdrant
scheme_count: 2
schemes:
- description: Authorization key, either read-write or read-only
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/qdrant-openapi-original.json
  type: apiKey
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/qdrant-openapi-original.json
  type: http
slug: qdrant-authentication
source_filename: qdrant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/qdrant-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Authorization key, either read-write or read-only\n  sources:\n  - openapi/qdrant-openapi-original.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/qdrant-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/authentication/qdrant-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Vector Databases
---
