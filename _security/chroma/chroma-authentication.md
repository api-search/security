---
api_key_in:
- header
api_specs:
- filename: chroma-collections-api-openapi.yml
  format: yaml
  label: Chroma Collections API
  slug: chroma-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroma/refs/heads/main/openapi/chroma-collections-api-openapi.yml
- filename: chroma-databases-api-openapi.yml
  format: yaml
  label: Chroma Databases API
  slug: chroma-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroma/refs/heads/main/openapi/chroma-databases-api-openapi.yml
- filename: chroma-records-api-openapi.yml
  format: yaml
  label: Chroma Records API
  slug: chroma-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroma/refs/heads/main/openapi/chroma-records-api-openapi.yml
- filename: chroma-search-api-openapi.yml
  format: yaml
  label: Chroma Search API
  slug: chroma-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroma/refs/heads/main/openapi/chroma-search-api-openapi.yml
- filename: chroma-system-api-openapi.yml
  format: yaml
  label: Chroma System API
  slug: chroma-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroma/refs/heads/main/openapi/chroma-system-api-openapi.yml
- filename: chroma-tenants-api-openapi.yml
  format: yaml
  label: Chroma Tenants API
  slug: chroma-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroma/refs/heads/main/openapi/chroma-tenants-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Chroma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chroma secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Chroma
provider_slug: chroma
scheme_count: 3
schemes:
- description: Bearer token authentication for Chroma Cloud. Obtain tokens from the Chroma Cloud dashboard.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/chroma-cloud-api-openapi.yml
  - openapi/chroma-server-api-openapi.yml
  type: http
- description: Static token authentication via the X-Chroma-Token header.
  in: header
  name: tokenAuth
  parameter: X-Chroma-Token
  sources:
  - openapi/chroma-server-api-openapi.yml
  type: apiKey
- description: HTTP Basic authentication using RFC 7617 with a user:password base64-encoded Authorization header.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/chroma-server-api-openapi.yml
  type: http
slug: chroma-authentication
source_filename: chroma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chroma-cloud-api-openapi.yml, openapi/chroma-server-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication for Chroma Cloud. Obtain tokens from the Chroma Cloud\n    dashboard.\n  sources:\n  - openapi/chroma-cloud-api-openapi.yml\n  - openapi/chroma-server-api-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: X-Chroma-Token\n  description: Static token authentication via the X-Chroma-Token header.\n  sources:\n  - openapi/chroma-server-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using RFC 7617 with a user:password base64-encoded\n    Authorization header.\n  sources:\n  - openapi/chroma-server-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chroma/refs/heads/main/authentication/chroma-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Artificial Intelligence
- AI-Native
- Apache 2.0
- Cloud
- Embeddings
- Hybrid Search
- JavaScript
- LLM
- Machine-Learning
- Multi-Modal
- Open-Source
- Python
- RAG
- Retrieval
- SDK
- Search
- Serverless
- TypeScript
- Vector Database
---
