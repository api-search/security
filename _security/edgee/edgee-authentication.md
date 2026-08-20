---
api_key_in:
- header
api_specs:
- filename: edgee-openapi-original.json
  format: json
  label: Edgee AI Gateway API
  slug: edgee-ai-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgee/refs/heads/main/openapi/edgee-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Edgee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Edgee secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Edgee
provider_slug: edgee
scheme_count: 5
schemes:
- applies_to: https://edgee.io
  bearerFormat: JWT
  description: Bearer authentication header of the form `Bearer <token>`, where `<token>` is your API key. More info [here](/docs/api-reference/authentication)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/edgee-openapi-original.json
  type: http
- applies_to: https://edgee.io
  description: Anthropic-style API key authentication using the x-api-key header
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/edgee-openapi-original.json
  type: apiKey
- applies_to: https://edgee.io
  description: 'Documented alternative to the bearer header: `-u <token>:` with a trailing colon so curl does not prompt for a password. The token goes in the username position.'
  in_openapi: false
  name: httpBasic
  scheme: basic
  sources:
  - https://www.edgee.ai/docs/api-reference/authentication
  type: http
- applies_to: https://edgee.io/v1/messages
  description: Claude CLI passthrough authentication. When set, the gateway uses this key instead of the Authorization header.
  in: header
  name: edgeeApiKeyPassthrough
  operation: createMessage
  parameter: x-edgee-api-key
  sources:
  - openapi/edgee-openapi-original.json
  type: apiKey
- applies_to: https://api.edgee.app
  description: 'Console API token, created in the Edgee Console under API Keys. Displayed once at creation and not retrievable afterwards. Observed token prefix in the docs examples: ek_live_.'
  env_var: EDGEE_CONSOLE_API_TOKEN
  failure_modes:
  - body: '{"error": "Unauthorized", "message": "Invalid or expired API token"}'
    status: 401
  - body: '{"error": "Forbidden", "message": "Your token does not have permission to access this resource"}'
    status: 403
  in_openapi: false
  name: consoleBearer
  scheme: bearer
  sources:
  - https://www.edgee.ai/docs/api-reference/console-api-setup
  type: http
slug: edgee-authentication
source_filename: edgee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: openapi/edgee-openapi-original.json\ndocs: https://www.edgee.ai/docs/api-reference/authentication\nnote: 'Baseline derived from the OpenAPI securitySchemes, then upgraded from the docs. Edgee runs TWO\n  separate credential systems on two hosts and says so explicitly in its own documentation: gateway\n  API keys for https://edgee.io, and Console tokens for https://api.edgee.app. They are not\n  interchangeable.'\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  https_required: true\n  credential_systems: 2\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer authentication header of the form `Bearer <token>`, where `<token>` is\n    your API key. More info [here](/docs/api-reference/authentication)\n  applies_to: https://edgee.io\n  sources:\n  - openapi/edgee-openapi-original.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n\
  \  parameter: x-api-key\n  description: Anthropic-style API key authentication using the x-api-key header\n  applies_to: https://edgee.io\n  sources:\n  - openapi/edgee-openapi-original.json\n- name: httpBasic\n  type: http\n  scheme: basic\n  description: 'Documented alternative to the bearer header: `-u <token>:` with a trailing colon so\n    curl does not prompt for a password. The token goes in the username position.'\n  applies_to: https://edgee.io\n  sources:\n  - https://www.edgee.ai/docs/api-reference/authentication\n  in_openapi: false\n- name: edgeeApiKeyPassthrough\n  type: apiKey\n  in: header\n  parameter: x-edgee-api-key\n  description: 'Claude CLI passthrough authentication. When set, the gateway uses this key instead of\n    the Authorization header.'\n  applies_to: https://edgee.io/v1/messages\n  operation: createMessage\n  sources:\n  - openapi/edgee-openapi-original.json\n- name: consoleBearer\n  type: http\n  scheme: bearer\n  description: 'Console API token, created\
  \ in the Edgee Console under API Keys. Displayed once at\n    creation and not retrievable afterwards. Observed token prefix in the docs examples: ek_live_.'\n  applies_to: https://api.edgee.app\n  sources:\n  - https://www.edgee.ai/docs/api-reference/console-api-setup\n  in_openapi: false\n  env_var: EDGEE_CONSOLE_API_TOKEN\n  failure_modes:\n  - {status: 401, body: '{\"error\": \"Unauthorized\", \"message\": \"Invalid or expired API token\"}'}\n  - {status: 403, body: '{\"error\": \"Forbidden\", \"message\": \"Your token does not have permission to\n        access this resource\"}'}\nkey_management:\n  console: https://www.edgee.ai/docs/quickstart/api-key\n  capabilities: [view tokens and creation dates, revoke immediately, rotate, monitor per-token usage]\n  api: https://www.edgee.ai/docs/api-reference/console-api-manage-gateway-api-keys\n  api_note: Gateway API keys can be created, listed, updated and deleted over the Console API.\n  scoping:\n  - {control: model and provider access,\
  \ source: 'https://www.edgee.ai/docs/features/model-access',\n    note: Which models and providers an organization may route to.}\n  - {control: usage limits, source: 'https://www.edgee.ai/docs/features/usage-limits', note: Spend\n      caps per key, per member or per squad over a daily, monthly or lifetime window.}\n  - {control: expiry, note: 'Keys can expire; an expired or inactive key returns 403 forbidden.'}\noauth:\n  api_oauth: false\n  cli_oauth: true\n  note: '`edgee auth login` opens a browser for OAuth-based login and writes credentials to\n    ~/.config/edgee/credentials.toml (mode 600). No authorization-server metadata is published —\n    /.well-known/oauth-authorization-server returns 404 on every Edgee host — so there is no\n    documented scope surface and no scopes/ artifact is emitted.'\nsso:\n  available: true\n  tier: Enterprise\n  methods: [SSO, SAML]\n  source: https://www.edgee.ai/pricing\nenv_vars:\n- {name: EDGEE_API_KEY, scope: gateway SDKs, source: 'https://www.edgee.ai/docs/sdk'}\n\
  - {name: EDGEE_CONSOLE_API_TOKEN, scope: Console API, source: 'https://www.edgee.ai/docs/api-reference/console-api-setup'}\n- {name: EDGEE_TOKEN, scope: legacy stdio MCP server, source: 'https://github.com/edgee-ai/mcp-server-edgee'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edgee/refs/heads/main/authentication/edgee-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Company
- Artificial Intelligence
- LLM
- AI Gateway
- Agents
- Developer Tools
- Observability
- FinOps
- Edge Computing
- Cost Management
---
