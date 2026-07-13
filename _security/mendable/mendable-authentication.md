---
api_key_in:
- query
api_specs:
- filename: mendable-openapi.yml
  format: yaml
  label: Mendable Chat & Answers API
  slug: mendable-chat-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendable/refs/heads/main/openapi/mendable-openapi.yml
- filename: mendable-openapi.yml
  format: yaml
  label: Mendable Conversations API
  slug: mendable-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendable/refs/heads/main/openapi/mendable-openapi.yml
- filename: mendable-openapi.yml
  format: yaml
  label: Mendable Data Ingestion & Sources API
  slug: mendable-data-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendable/refs/heads/main/openapi/mendable-openapi.yml
- filename: mendable-openapi.yml
  format: yaml
  label: Mendable Ratings API
  slug: mendable-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendable/refs/heads/main/openapi/mendable-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mendable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mendable secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mendable
provider_slug: mendable
scheme_count: 2
schemes:
- description: Mendable api_key. Sent as the api_key field inside the JSON request body for every endpoint (modeled here as apiKey for tooling).
  in: query
  name: apiKeyBody
  parameter: api_key
  sources:
  - openapi/mendable-openapi.yml
  type: apiKey
- description: Mendable api_key supplied as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mendable-openapi.yml
  type: http
slug: mendable-authentication
source_filename: mendable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mendable-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyBody\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Mendable api_key. Sent as the api_key field inside the JSON request body for\n    every endpoint (modeled here as apiKey for tooling).\n  sources:\n  - openapi/mendable-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Mendable api_key supplied as a Bearer token in the Authorization header.\n  sources:\n  - openapi/mendable-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mendable/refs/heads/main/authentication/mendable-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI
- Answers
- Enterprise Search
- RAG
- Support
---
