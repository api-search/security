---
api_key_in:
- header
api_specs:
- filename: qdrant-openapi-original.json
  format: json
  label: Qdrant API
  slug: qdrant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-openapi-original.json
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
- AI
- Artificial Intelligence
- Vector Databases
---
