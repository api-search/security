---
api_key_in:
- header
api_specs:
- filename: nuclia-openapi.yml
  format: yaml
  label: Nuclia Knowledge Boxes API
  slug: knowledge-boxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/openapi/nuclia-openapi.yml
- filename: nuclia-openapi.yml
  format: yaml
  label: Nuclia Resources & Ingestion API
  slug: resources-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/openapi/nuclia-openapi.yml
- filename: nuclia-openapi.yml
  format: yaml
  label: Nuclia Search & Find API
  slug: search-find-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/openapi/nuclia-openapi.yml
- filename: nuclia-openapi.yml
  format: yaml
  label: Nuclia Ask & Chat (RAG) API
  slug: ask-chat-rag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/openapi/nuclia-openapi.yml
- filename: nuclia-openapi.yml
  format: yaml
  label: Nuclia Predict (NUA) API
  slug: predict-nua-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/openapi/nuclia-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nuclia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nuclia secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nuclia
provider_slug: nuclia
scheme_count: 3
schemes:
- description: 'Knowledge Box service account API key. Pass as `X-NUCLIA-SERVICEACCOUNT: Bearer <token>`. Reader keys allow search/find/ask, Writer keys allow ingestion and resource modification, Manager keys allow administration. Public search endpoints may be called without a key when the Knowledge Box is public.'
  in: header
  name: apiKey
  parameter: X-NUCLIA-SERVICEACCOUNT
  sources:
  - openapi/nuclia-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: OAuth2 / account bearer token obtained from the Nuclia authentication service, used by the dashboard and management endpoints.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nuclia-openapi.yml
  type: http
- description: 'Nuclia Understanding API (NUA) key. Pass as `X-NUCLIA-NUAKEY: Bearer <token>` to call the /v1/predict endpoints.'
  in: header
  name: nuaKey
  parameter: X-NUCLIA-NUAKEY
  sources:
  - openapi/nuclia-openapi.yml
  type: apiKey
slug: nuclia-authentication
source_filename: nuclia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nuclia-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-NUCLIA-SERVICEACCOUNT\n  description: 'Knowledge Box service account API key. Pass as `X-NUCLIA-SERVICEACCOUNT: Bearer\n    <token>`. Reader keys allow search/find/ask, Writer keys allow ingestion and resource modification,\n    Manager keys allow administration. Public search endpoints may be called without a key when\n    the Knowledge Box is public.'\n  sources:\n  - openapi/nuclia-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 / account bearer token obtained from the Nuclia authentication service,\n    used by the dashboard and management endpoints.\n  sources:\n  - openapi/nuclia-openapi.yml\n- name: nuaKey\n  type: apiKey\n  in: header\n  parameter: X-NUCLIA-NUAKEY\n  description: 'Nuclia Understanding\
  \ API (NUA) key. Pass as `X-NUCLIA-NUAKEY: Bearer <token>`\n    to call the /v1/predict endpoints.'\n  sources:\n  - openapi/nuclia-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/authentication/nuclia-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- AI
- RAG
- Search
- Knowledge Base
- Unstructured Data
---
