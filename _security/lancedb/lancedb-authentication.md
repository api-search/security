---
api_key_in:
- header
api_specs:
- filename: lance-namespace-openapi.yaml
  format: yaml
  label: LanceDB OSS
  slug: oss
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancedb/main/openapi/lance-namespace-openapi.yaml
- filename: lance-namespace-openapi.yaml
  format: yaml
  label: LanceDB Cloud
  slug: cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancedb/main/openapi/lance-namespace-openapi.yaml
- filename: spec.yaml
  format: yaml
  label: Lance Namespace Specification
  slug: lance-namespace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/lance-format/lance-namespace/main/docs/src/spec.yaml
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
- Multimodal
- Lance Format
- Lakehouse
- RAG
- Agent Memory
- Open Source
- Embeddings
- Full-Text Search
- Hybrid Search
- Columnar Storage
- Arrow
- AI Infrastructure
---
