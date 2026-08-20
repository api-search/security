---
api_key_in:
- header
api_specs:
- filename: lancedb-data-api-openapi.yml
  format: yaml
  label: LanceDB Data API
  slug: lancedb-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancedb/refs/heads/main/openapi/lancedb-data-api-openapi.yml
- filename: lancedb-index-api-openapi.yml
  format: yaml
  label: LanceDB Index API
  slug: lancedb-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancedb/refs/heads/main/openapi/lancedb-index-api-openapi.yml
- filename: lancedb-materializedview-api-openapi.yml
  format: yaml
  label: LanceDB MaterializedView API
  slug: lancedb-materializedview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancedb/refs/heads/main/openapi/lancedb-materializedview-api-openapi.yml
- filename: lancedb-metadata-api-openapi.yml
  format: yaml
  label: LanceDB Metadata API
  slug: lancedb-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancedb/refs/heads/main/openapi/lancedb-metadata-api-openapi.yml
- filename: lancedb-namespace-api-openapi.yml
  format: yaml
  label: LanceDB Namespace API
  slug: lancedb-namespace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancedb/refs/heads/main/openapi/lancedb-namespace-api-openapi.yml
- filename: lancedb-table-api-openapi.yml
  format: yaml
  label: LanceDB Table API
  slug: lancedb-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancedb/refs/heads/main/openapi/lancedb-table-api-openapi.yml
- filename: lancedb-tag-api-openapi.yml
  format: yaml
  label: LanceDB Tag API
  slug: lancedb-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancedb/refs/heads/main/openapi/lancedb-tag-api-openapi.yml
- filename: lancedb-transaction-api-openapi.yml
  format: yaml
  label: LanceDB Transaction API
  slug: lancedb-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancedb/refs/heads/main/openapi/lancedb-transaction-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Lancedb Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: LanceDB secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: LanceDB
provider_slug: lancedb
scheme_count: 3
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /oauth/token
  name: OAuth2
  sources:
  - openapi/lance-namespace-openapi.yaml
  type: oauth2
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/lance-namespace-openapi.yaml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/lance-namespace-openapi.yaml
  type: apiKey
slug: lancedb-authentication
source_filename: lancedb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lance-namespace-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n    scopes: 0\n  sources:\n  - openapi/lance-namespace-openapi.yaml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/lance-namespace-openapi.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/lance-namespace-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lancedb/refs/heads/main/authentication/lancedb-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Vector Database
- Multi-Modal
- Lance Format
- Lakehouse
- RAG
- Agent Memory
- Open-Source
- Embeddings
- Full-Text Search
- Hybrid Search
- Columnar Storage
- Arrow
- AI Infrastructure
---
