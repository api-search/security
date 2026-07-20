---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Co Create Authentication
name_suffix: Authentication
oauth_flows: []
overview: Co:Create secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Co:Create
provider_slug: co-create
scheme_count: 1
schemes:
- description: 'All API requests must include the Secret API Key as a Bearer token — `Authorization: Bearer <YOUR_KEY>`. Keys are generated per team in Team Settings. Separate keys exist per environment (sandbox vs production); the production key is a secret and must never be exposed to frontend code or end users.'
  environments:
  - base_url: https://api.cocrt.xyz
    name: production
  - base_url: https://api.testcocrt.xyz
    name: sandbox
  format: Bearer <YOUR_KEY_HERE>
  header: Authorization
  name: SecretApiKey
  scheme: bearer
  sources:
  - https://docs.usecocreate.io/docs/sandbox-vs-production-environment
  type: http
slug: co-create-authentication
source_filename: co-create-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.usecocreate.io/docs/sandbox-vs-production-environment\ndocs: https://docs.usecocreate.io/docs/authentication-and-api-keys\nnote: >-\n  Captured from Co:Create's own published documentation via the Internet Archive; the live docs host no longer\n  resolves. Server-to-server API calls authenticate with a static Secret API Key passed as an HTTP Bearer token\n  in the Authorization header. Separately, end-user identity in client apps is handled via \"Authentication with\n  Dynamic Tokens\" (Dynamic, dynamic.xyz) — that governs wallet/user sign-in, not the REST API credential.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: SecretApiKey\n  type: http\n  scheme: bearer\n  description: >-\n    All API requests must include the Secret API Key as a Bearer token — `Authorization: Bearer <YOUR_KEY>`.\n    Keys are generated per team in Team Settings. Separate\
  \ keys exist per environment (sandbox vs production);\n    the production key is a secret and must never be exposed to frontend code or end users.\n  header: Authorization\n  format: 'Bearer <YOUR_KEY_HERE>'\n  environments:\n  - name: production\n    base_url: https://api.cocrt.xyz\n  - name: sandbox\n    base_url: https://api.testcocrt.xyz\n  sources:\n  - https://docs.usecocreate.io/docs/sandbox-vs-production-environment\nend_user_identity:\n  name: Dynamic Tokens\n  provider: Dynamic (dynamic.xyz)\n  description: >-\n    Client-side end-user authentication / wallet sign-in for token-driven communities, documented as\n    \"Authentication with Dynamic Tokens\". Distinct from the server-side Secret API Key.\n  docs: https://docs.usecocreate.io/docs/dynamic-cocreate-authentication-guide\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/co-create/refs/heads/main/authentication/co-create-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Web3
- Loyalty
- Rewards
- NFT
- Blockchain
- Polygon
- Tokens
- Community
- Crypto
---
