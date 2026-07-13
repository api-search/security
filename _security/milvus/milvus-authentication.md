---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Milvus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Milvus secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Milvus
provider_slug: milvus
scheme_count: 1
schemes:
- description: 'Bearer token of the form `username:password` (e.g. `root:milvus`) when

    authentication is enabled.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/milvus-openapi.yml
  type: http
slug: milvus-authentication
source_filename: milvus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/milvus-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer token of the form `username:password` (e.g. `root:milvus`) when\n    authentication is enabled.\n  sources:\n  - openapi/milvus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/milvus/refs/heads/main/authentication/milvus-authentication.yml
summary_line: http · 1 scheme
tags:
- Vector Database
- AI
- Embeddings
- Open Source
- Cloud-Native
---
