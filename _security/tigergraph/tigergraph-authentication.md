---
api_key_in: []
api_specs:
- filename: tigergraph-authentication-api-openapi.yml
  format: yaml
  label: TigerGraph Authentication API
  slug: tigergraph-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/openapi/tigergraph-authentication-api-openapi.yml
- filename: tigergraph-data-api-openapi.yml
  format: yaml
  label: TigerGraph Data API
  slug: tigergraph-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/openapi/tigergraph-data-api-openapi.yml
- filename: tigergraph-query-api-openapi.yml
  format: yaml
  label: TigerGraph Query API
  slug: tigergraph-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/openapi/tigergraph-query-api-openapi.yml
- filename: tigergraph-schema-api-openapi.yml
  format: yaml
  label: TigerGraph Schema API
  slug: tigergraph-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/openapi/tigergraph-schema-api-openapi.yml
- filename: tigergraph-system-api-openapi.yml
  format: yaml
  label: TigerGraph System API
  slug: tigergraph-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/openapi/tigergraph-system-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tigergraph Authentication
name_suffix: Authentication
oauth_flows: []
overview: TigerGraph secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TigerGraph
provider_slug: tigergraph
scheme_count: 1
schemes:
- description: Bearer token obtained from POST /restpp/requesttoken (required only when token authentication is enabled on the TigerGraph server).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tigergraph-openapi.yml
  type: http
slug: tigergraph-authentication
source_filename: tigergraph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tigergraph-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from POST /restpp/requesttoken (required only when token\n    authentication is enabled on the TigerGraph server).\n  sources:\n  - openapi/tigergraph-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/authentication/tigergraph-authentication.yml
summary_line: http · 1 scheme
tags:
- Graph Database
- Analytics
- GSQL
- REST++
- Graph Analytics
---
