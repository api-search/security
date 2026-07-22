---
api_key_in:
- header
auth_types:
- apiKey
description: The Maisa REST API (base URL https://api.maisa.ai) authenticates with a static API key sent in a custom X-API-Key request header. The official SDKs read the key from the MAISA_API_KEY environment variable or an api_key constructor argument. There is no public OAuth/OIDC surface on the API host; the docs portal (docs.maisa.ai) itself sits behind an AWS Cognito login, but the API is key-authenticated. No OpenAPI securitySchemes block is publicly available (docs are gated), so this profile is derived from the official client libraries rather than a published spec.
kind: authentication
layout: security
method: searched
name: Maisa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maisa secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Maisa
provider_slug: maisa
scheme_count: 1
schemes:
- env_var: MAISA_API_KEY
  in: header
  name: apiKeyHeader
  parameter_name: X-API-Key
  sources:
  - https://github.com/maisaai/python-sdk
  - https://github.com/maisaai/node-sdk
  type: apiKey
slug: maisa-authentication
source_filename: maisa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/maisaai/python-sdk\ndocs: https://docs.maisa.ai/docs/sdk\ndescription: >-\n  The Maisa REST API (base URL https://api.maisa.ai) authenticates with a\n  static API key sent in a custom X-API-Key request header. The official SDKs\n  read the key from the MAISA_API_KEY environment variable or an api_key\n  constructor argument. There is no public OAuth/OIDC surface on the API host;\n  the docs portal (docs.maisa.ai) itself sits behind an AWS Cognito login, but\n  the API is key-authenticated. No OpenAPI securitySchemes block is publicly\n  available (docs are gated), so this profile is derived from the official\n  client libraries rather than a published spec.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: apiKeyHeader\n    type: apiKey\n    in: header\n    parameter_name: X-API-Key\n    env_var: MAISA_API_KEY\n    sources: [https://github.com/maisaai/python-sdk,\
  \ https://github.com/maisaai/node-sdk]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maisa/refs/heads/main/authentication/maisa-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai
- Agentic AI
- AI Agents
- Digital Workers
- Business Process Automation
- Enterprise Automation
- Banking
- Insurance
---
