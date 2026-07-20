---
api_key_in:
- header
- env
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Imandra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Imandra secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Imandra
provider_slug: imandra
scheme_count: 1
schemes:
- description: Imandra Universe API key. Obtain a free key by signing up at https://universe.imandra.ai, then set the IMANDRA_UNI_KEY environment variable. The key authenticates the imandra Python client, the codelogician CLI, and the CodeLogician MCP server against the hosted Imandra Universe / ImandraX reasoning services.
  env: IMANDRA_UNI_KEY
  in: header
  name: ImandraUniverseApiKey
  sources:
  - https://codelogician.dev/docs/getting-started/
  type: apiKey
slug: imandra-authentication
source_filename: imandra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://codelogician.dev/docs/getting-started/, https://universe.imandra.ai\ndocs: https://codelogician.dev/docs/getting-started/\nsummary:\n  types: [apiKey]\n  api_key_in: [header, env]\nschemes:\n  - name: ImandraUniverseApiKey\n    type: apiKey\n    in: header\n    env: IMANDRA_UNI_KEY\n    description: >-\n      Imandra Universe API key. Obtain a free key by signing up at\n      https://universe.imandra.ai, then set the IMANDRA_UNI_KEY environment\n      variable. The key authenticates the imandra Python client, the\n      codelogician CLI, and the CodeLogician MCP server against the hosted\n      Imandra Universe / ImandraX reasoning services.\n    sources: [https://codelogician.dev/docs/getting-started/]\nnotes: >-\n  Imandra Universe uses an API-key model (no OAuth scope surface documented),\n  so no scopes/ artifact is emitted. The self-hosted ImandraX gRPC API\n  (see grpc/) uses session-based access via the SessionManager\
  \ service.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imandra/refs/heads/main/authentication/imandra-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai
- Automated Reasoning
- Formal Verification
- Theorem Proving
- Developer Tools
- Code Analysis
- Financial Services
- gRPC
- MCP
---
