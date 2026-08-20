---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fiddlerai Authentication
name_suffix: Authentication
oauth_flows: []
overview: fiddler.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: fiddler.ai
provider_slug: fiddlerai
scheme_count: 1
schemes:
- location: 'Authorization: Bearer <token>'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.fiddler.ai/api/rest-api/rest-api
  token_type: personal access token / API key (user-access-key)
  type: http
slug: fiddlerai-authentication
source_filename: fiddlerai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.fiddler.ai/api/rest-api/rest-api\ndocs: https://docs.fiddler.ai/developers/python-client-guides/installation-and-setup\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\nnotes: >-\n  All Fiddler REST API and MCP endpoints require Bearer token authentication.\n  Tokens are personal access tokens / API keys minted per user from the Fiddler\n  deployment (Settings > Credentials), scoped by the user's RBAC role. The Python\n  client authenticates with the deployment URL plus the same token.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    location: 'Authorization: Bearer <token>'\n    token_type: personal access token / API key (user-access-key)\n    sources: [https://docs.fiddler.ai/api/rest-api/rest-api]\naccess_control:\n  model: RBAC\n  note: Authorization is role-based; the user-access-keys / users endpoints manage keys and role assignments.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiddlerai/refs/heads/main/authentication/fiddlerai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI Observability
- Machine-Learning
- LLM
- Model Monitoring
- Guardrails
- MLOps
- AI Governance
- Explainability
- Agent Observability
- AI Security
---
