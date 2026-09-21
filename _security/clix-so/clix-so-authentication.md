---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: clix-so-openapi.yml
  format: yaml
  label: Clix External API
  slug: clix-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clix-so/refs/heads/main/openapi/clix-so-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Clix So Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clix secures its APIs with apiKey across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clix
provider_slug: clix-so
scheme_count: 5
schemes:
- description: Project ID for authentication — identifies the project; rate limits are tracked on it.
  in: header
  name: ProjectIdAuth
  parameter: X-Clix-Project-ID
  required_with: ApiKeyAuth
  sources:
  - openapi/clix-so-openapi.yml
  - https://docs.clix.so/api-reference/overview
  surfaces:
  - REST
  type: apiKey
- description: API Key for authentication — public or secret depending on the operation.
  in: header
  key_types:
  - kind: public
    prefix: not stated
    use: Client-side SDKs in mobile apps, browsers, or public environments
    visibility: Safe to expose
  - kind: secret
    prefix: clix_sk_
    use: Server-to-server communication, secure backend operations — user management, message sending, campaign triggering
    visibility: Must keep confidential
  name: ApiKeyAuth
  parameter: X-Clix-API-Key
  sources:
  - openapi/clix-so-openapi.yml
  - https://docs.clix.so/api-reference/overview
  surfaces:
  - REST
  type: apiKey
- description: Secret API key for A2A authentication (agent card securitySchemes.apiKey). Secret keys only; public keys are rejected; the project is resolved from the key so no project header is sent.
  in: header
  name: apiKey (A2A)
  observed: POST /a2a without the header -> 401 text/plain "Missing API key" (2026-09-19)
  parameter: X-API-Key
  sources:
  - a2a/clix-so-agent-card.json
  - https://docs.clix.so/a2a/overview
  surfaces:
  - A2A — POST https://api.clix.so/a2a
  type: apiKey
- description: Neither MCP server takes a credential — the stdio @clix-so/clix-mcp-server and the Mintlify docs endpoint at https://docs.clix.so/mcp both search public documentation only.
  name: none (MCP)
  surfaces:
  - MCP
  type: none
- description: '`clix login` authenticates the CLI with a Clix account via device flow; `clix logout` removes stored credentials; `clix whoami` shows the user. A developer-session login, not an API scheme.'
  name: device flow (CLI)
  sources:
  - https://docs.clix.so/clix-cli
  surfaces:
  - CLI
  type: human-login
slug: clix-so-authentication
source_filename: clix-so-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://docs.clix.so/api-reference/overview\nderived_from: openapi/clix-so-openapi.yml\ndocs:\n- https://docs.clix.so/api-reference/overview\n- https://docs.clix.so/a2a/overview\n- https://docs.clix.so/clix-cli\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2: false\n  oidc: false\n  mtls: false\n  note: >-\n    Static API keys throughout. REST needs two headers on every call (project id + key); A2A needs one\n    (secret key, from which the project is resolved). Two key TYPES exist — public for client SDKs, secret\n    (clix_sk_ prefix) for server-side writes — and the docs are explicit that public keys are rejected on\n    /a2a and should not be used for user management, sending or triggering. Keys are issued in the console\n    (console.clix.so, login-gated); no OAuth metadata is served on any host.\nschemes:\n- name: ProjectIdAuth\n  type: apiKey\n  in: header\n  parameter: X-Clix-Project-ID\n  description:\
  \ Project ID for authentication — identifies the project; rate limits are tracked on it.\n  required_with: ApiKeyAuth\n  surfaces: [REST]\n  sources: [openapi/clix-so-openapi.yml, 'https://docs.clix.so/api-reference/overview']\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Clix-API-Key\n  description: API Key for authentication — public or secret depending on the operation.\n  key_types:\n  - {kind: public, prefix: not stated, use: 'Client-side SDKs in mobile apps, browsers, or public environments', visibility: Safe to expose}\n  - {kind: secret, prefix: clix_sk_, use: 'Server-to-server communication, secure backend operations — user management, message sending, campaign triggering', visibility: Must keep confidential}\n  surfaces: [REST]\n  sources: [openapi/clix-so-openapi.yml, 'https://docs.clix.so/api-reference/overview']\n- name: apiKey (A2A)\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Secret API key for A2A authentication (agent card securitySchemes.apiKey).\
  \ Secret keys only; public keys are rejected; the project is resolved from the key so no project header is sent.\n  surfaces: [A2A — POST https://api.clix.so/a2a]\n  sources: [a2a/clix-so-agent-card.json, 'https://docs.clix.so/a2a/overview']\n  observed: 'POST /a2a without the header -> 401 text/plain \"Missing API key\" (2026-09-19)'\n- name: none (MCP)\n  type: none\n  description: Neither MCP server takes a credential — the stdio @clix-so/clix-mcp-server and the Mintlify docs endpoint at https://docs.clix.so/mcp both search public documentation only.\n  surfaces: [MCP]\n- name: device flow (CLI)\n  type: human-login\n  description: '`clix login` authenticates the CLI with a Clix account via device flow; `clix logout` removes stored credentials; `clix whoami` shows the user. A developer-session login, not an API scheme.'\n  surfaces: [CLI]\n  sources: ['https://docs.clix.so/clix-cli']\nkey_management:\n  issued_in: Clix console (https://console.clix.so — every path 307s to /auth/login)\n\
  \  rotation: 'Docs advise: store keys in environment variables or a secrets manager, rotate, least privilege (public in clients, secret only in trusted backends), audit and revoke unused keys, alert on unusual activity. No rotation API is documented.'\n  scopes: none — no scoped or restricted keys beyond the public/secret split\nerrors:\n  '401': 'Verify API key and Project ID are correct and valid. Observed bodies: \"Missing project id\" (REST), \"Missing API key\" (A2A).'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clix-so/refs/heads/main/authentication/clix-so-authentication.yml
summary_line: apiKey · 5 schemes
tags:
- Push Notifications
- Mobile
- Messaging
- Campaigns
- Event Tracking
- Customer Engagement
- A2A
- MCP
- Agents
- SDK
- United States
- Company
---
