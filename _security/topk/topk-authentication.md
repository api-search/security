---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Topk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Topk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Topk
provider_slug: topk
scheme_count: 1
schemes:
- applies_to:
  - REST API (collections, datasets, management)
  - Python SDK (topk-sdk)
  - JavaScript SDK (topk-js)
  - Rust SDK (topk-rs)
  - SQL / PostgreSQL wire protocol
  - CLI (topk login / TOPK_API_KEY)
  - MCP server
  description: 'All TopK access (REST API, SDKs, CLI, and the MCP server) authenticates with a TopK API key presented as a Bearer token in the Authorization header, or supplied via the TOPK_API_KEY environment variable. API keys are generated in the TopK console (console.topk.io). Requests are region-scoped: the client is configured with both an API key and a region (e.g. aws-us-east-1-elastica) which selects the {region}.api.topk.io host.'
  env_var: TOPK_API_KEY
  header: Authorization
  in: header
  key_management_url: https://console.topk.io
  name: apiKeyBearer
  scheme: bearer
  type: http
  value_format: Bearer <TOPK_API_KEY>
slug: topk-authentication
source_filename: topk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.topk.io/sdk/topk-py/overview + https://docs.topk.io/mcp-server + https://docs.topk.io/cli\ndocs: https://docs.topk.io\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_env: TOPK_API_KEY\n  oauth2_flows: []\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  description: >-\n    All TopK access (REST API, SDKs, CLI, and the MCP server) authenticates with a TopK API key\n    presented as a Bearer token in the Authorization header, or supplied via the TOPK_API_KEY\n    environment variable. API keys are generated in the TopK console (console.topk.io). Requests\n    are region-scoped: the client is configured with both an API key and a region (e.g.\n    aws-us-east-1-elastica) which selects the {region}.api.topk.io host.\n  in: header\n  header: Authorization\n  value_format: 'Bearer <TOPK_API_KEY>'\n  env_var: TOPK_API_KEY\n  key_management_url: https://console.topk.io\n  applies_to:\n\
  \  - REST API (collections, datasets, management)\n  - Python SDK (topk-sdk)\n  - JavaScript SDK (topk-js)\n  - Rust SDK (topk-rs)\n  - SQL / PostgreSQL wire protocol\n  - CLI (topk login / TOPK_API_KEY)\n  - MCP server\nnotes: No OAuth2 or OpenID Connect surface is documented; TopK uses opaque API-key bearer tokens. No public OpenAPI is published, so this profile is sourced from the SDK/CLI/MCP documentation rather than derived from a spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/topk/refs/heads/main/authentication/topk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Search
- Vector Search
- Hybrid Search
- Multi-Vector Retrieval
- Semantic Search
- BM25
- Retrieval
- RAG
- Question Answering
- AI Infrastructure
- Embeddings
- MCP
---
