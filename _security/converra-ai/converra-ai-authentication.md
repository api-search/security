---
anonymous_access: false
api_key_in: []
api_specs:
- filename: converra-ai-api-openapi-generated.yml
  format: yaml
  label: Converra API Reference API
  slug: api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converra-ai/openapi/_ae-authored/converra-ai-api-openapi-generated.yml
- filename: converra-ai-core-openapi-generated.yml
  format: yaml
  label: Converra core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converra-ai/openapi/_ae-authored/converra-ai-core-openapi-generated.yml
- filename: converra-ai-guide-openapi-generated.yml
  format: yaml
  label: Converra Guide API
  slug: guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/converra-ai/openapi/_ae-authored/converra-ai-guide-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Converra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Converra declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Converra
provider_slug: converra-ai
scheme_count: 1
schemes:
- applies_to:
  - REST API https://converra.ai/api/v1
  - MCP server https://converra.ai/api/mcp
  description: All API requests require authentication using an API key, sent in the Authorization header as a Bearer token. Keys are created under Integrations → API Keys in the workspace and shown only once.
  format: 'Authorization: Bearer sk_live_your_api_key_here'
  header: Authorization
  in: header
  key_prefixes:
  - environment: Production
    prefix: sk_live_
  - environment: Development/Testing
    prefix: sk_test_
  name: bearerApiKey
  scheme: bearer
  type: http
slug: converra-ai-authentication
source_filename: converra-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://converra.ai/docs/api/authentication\ndocs: https://converra.ai/docs/api/authentication\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer sk_live_your_api_key_here'\n  description: All API requests require authentication using an API key, sent in the Authorization header as a Bearer token. Keys are created under Integrations → API Keys in the workspace and shown only once.\n  key_prefixes:\n  - prefix: sk_live_\n    environment: Production\n  - prefix: sk_test_\n    environment: Development/Testing\n  applies_to:\n  - REST API https://converra.ai/api/v1\n  - MCP server https://converra.ai/api/mcp\nkey_management:\n  creation: Integrations → API Keys → Create API Key (key only shown once)\n  revocation: Integrations → API Keys → Revoke; requests using a revoked key immediately fail\n  rotation: Create a new key before revoking the old\
  \ one to rotate without downtime\n  expiry: Keys can expire (\"API key has expired\" 401 error documented)\nerrors:\n- status: 401\n  code: UNAUTHORIZED\n  message: Invalid API key\n- status: 401\n  code: UNAUTHORIZED\n  message: Authorization header required\n- status: 401\n  code: UNAUTHORIZED\n  message: API key has expired\noauth2: false\nnote: No OAuth flows or scopes are documented; scopes/ not written.\n"
source_yaml_url: https://artifacts.apis.io/converra-ai/authentication/converra-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agent Optimization
- LLM Observability
- Simulation Testing
- Prompt Engineering
- MCP
---
