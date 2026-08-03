---
api_key_in:
- header
api_specs:
- filename: aleph-alpha-pharia-inference-openapi.json
  format: json
  label: PhariaInference API
  slug: pharia-inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-pharia-inference-openapi.json
- filename: aleph-alpha-pharia-data-openapi.json
  format: json
  label: PhariaData API
  slug: pharia-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-pharia-data-openapi.json
- filename: aleph-alpha-pharia-search-openapi.json
  format: json
  label: PhariaSearch / Document Index API
  slug: pharia-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-pharia-search-openapi.json
- filename: aleph-alpha-pharia-studio-openapi.json
  format: json
  label: PhariaStudio API
  slug: pharia-studio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-pharia-studio-openapi.json
- filename: aleph-alpha-pharia-os-openapi.json
  format: json
  label: PhariaOS Manager API
  slug: pharia-os
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-pharia-os-openapi.json
- filename: aleph-alpha-responses-openapi.json
  format: json
  label: Responses API (Stateful Responses)
  slug: responses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-responses-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aleph Alpha Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aleph Alpha secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Aleph Alpha
provider_slug: aleph-alpha
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: Bearer
  scheme: bearer
  sources:
  - openapi/aleph-alpha-pharia-data-openapi.json
  - openapi/aleph-alpha-pharia-inference-openapi.json
  - openapi/aleph-alpha-pharia-search-openapi.json
  - openapi/aleph-alpha-pharia-studio-openapi.json
  - openapi/aleph-alpha-responses-openapi.json
  type: http
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/aleph-alpha-pharia-os-openapi.json
  type: apiKey
slug: aleph-alpha-authentication
source_filename: aleph-alpha-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/aleph-alpha-pharia-data-openapi.json, openapi/aleph-alpha-pharia-inference-openapi.json,\n  openapi/aleph-alpha-pharia-os-openapi.json, openapi/aleph-alpha-pharia-search-openapi.json,\n  openapi/aleph-alpha-pharia-studio-openapi.json, openapi/aleph-alpha-responses-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/aleph-alpha-pharia-data-openapi.json\n  - openapi/aleph-alpha-pharia-inference-openapi.json\n  - openapi/aleph-alpha-pharia-search-openapi.json\n  - openapi/aleph-alpha-pharia-studio-openapi.json\n  - openapi/aleph-alpha-responses-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/aleph-alpha-pharia-os-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/authentication/aleph-alpha-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Large Language Models
- Generative AI
- Sovereign AI
- Inference
- Embeddings
- Semantic Search
- Vector Search
- Agents
- Model Context Protocol
- Germany
- Enterprise Software
- Government
---
