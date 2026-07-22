---
api_key_in: []
api_specs:
- filename: zeroentropy-openapi.json
  format: json
  label: ZeroEntropy API
  slug: zeroentropy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeroentropy/refs/heads/main/openapi/zeroentropy-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zeroentropy Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZeroEntropy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ZeroEntropy
provider_slug: zeroentropy
scheme_count: 1
schemes:
- description: 'The `Authorization` header must be provided in the format `Bearer <your-api-key>`.


    You can get your API Key at the [Dashboard](https://dashboard.zeroentropy.dev/)!'
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/zeroentropy-openapi.json
  type: http
slug: zeroentropy-authentication
source_filename: zeroentropy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/zeroentropy-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  description: |-\n    The `Authorization` header must be provided in the format `Bearer <your-api-key>`.\n\n    You can get your API Key at the [Dashboard](https://dashboard.zeroentropy.dev/)!\n  sources:\n  - openapi/zeroentropy-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeroentropy/refs/heads/main/authentication/zeroentropy-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise Saas
- Artificial Intelligence
- Search
- Retrieval
- Embeddings
- Reranking
- RAG
---
