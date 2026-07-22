---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Sensoai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Senso.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Senso.ai
provider_slug: sensoai
scheme_count: 1
schemes:
- description: All Senso Org API requests authenticate with an API key passed in the X-API-Key request header. Keys are scoped to an organization and created/managed via the dashboard or the api-keys API. The CLI resolves the key from --api-key, the SENSO_API_KEY env var, or a stored config file. Docs describe API key scoping, headers, and best practices.
  in: header
  key_prefix: tgr_
  name: ApiKeyAuth
  parameter_name: X-API-Key
  sources:
  - https://docs.senso.ai/docs/authentication
  - https://github.com/AI-Template-SDK/senso-user-cli
  type: apiKey
slug: sensoai-authentication
source_filename: sensoai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.senso.ai/docs/authentication\ndocs: https://docs.senso.ai/docs/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  key_prefix: tgr_\n  description: >-\n    All Senso Org API requests authenticate with an API key passed in the X-API-Key request\n    header. Keys are scoped to an organization and created/managed via the dashboard or the\n    api-keys API. The CLI resolves the key from --api-key, the SENSO_API_KEY env var, or a\n    stored config file. Docs describe API key scoping, headers, and best practices.\n  sources:\n  - https://docs.senso.ai/docs/authentication\n  - https://github.com/AI-Template-SDK/senso-user-cli\nnotes: >-\n  The end-user dashboard (app.senso.ai / docs.senso.ai) uses Clerk for interactive sign-in\n  (publishable key pk_live_ at clerk.senso.ai), but programmatic\
  \ API access is key-based\n  (X-API-Key). No OAuth 2.0 / OIDC scheme is documented for the API, so no OAuth scopes artifact\n  is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensoai/refs/heads/main/authentication/sensoai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Knowledge Base
- AI Agents
- Content Generation
- Semantic Search
- Generative Engine Optimization
- Verified Context
- Agentic Web
- MCP
---
