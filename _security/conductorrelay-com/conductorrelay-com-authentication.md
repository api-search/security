---
anonymous_access: false
api_key_in: []
api_specs:
- filename: conductorrelay-com-a2a-network-api-openapi.yml
  format: yaml
  label: Conductor Relay A2A Network API
  slug: conductorrelay-com-a2a-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-a2a-network-api-openapi.yml
- filename: conductorrelay-com-agent-feedback-api-openapi.yml
  format: yaml
  label: Conductor Relay Agent Feedback API
  slug: conductorrelay-com-agent-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-agent-feedback-api-openapi.yml
- filename: conductorrelay-com-agent-funding-api-openapi.yml
  format: yaml
  label: Conductor Relay Agent Funding API
  slug: conductorrelay-com-agent-funding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-agent-funding-api-openapi.yml
- filename: conductorrelay-com-agent-identity-onboarding-api-openapi.yml
  format: yaml
  label: Conductor Relay Agent Identity & Onboarding API
  slug: conductorrelay-com-agent-identity-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-agent-identity-onboarding-api-openapi.yml
- filename: conductorrelay-com-agent-performance-network-api-openapi.yml
  format: yaml
  label: Conductor Relay Agent Performance Network API
  slug: conductorrelay-com-agent-performance-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-agent-performance-network-api-openapi.yml
- filename: conductorrelay-com-agents-api-openapi.yml
  format: yaml
  label: Conductor Relay Agents API
  slug: conductorrelay-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-agents-api-openapi.yml
- filename: conductorrelay-com-capabilities-api-openapi.yml
  format: yaml
  label: Conductor Relay Capabilities API
  slug: conductorrelay-com-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-capabilities-api-openapi.yml
- filename: conductorrelay-com-direct-session-exchange-api-openapi.yml
  format: yaml
  label: Conductor Relay Direct Session Exchange API
  slug: conductorrelay-com-direct-session-exchange-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-direct-session-exchange-api-openapi.yml
- filename: conductorrelay-com-faucet-api-openapi.yml
  format: yaml
  label: Conductor Relay Faucet API
  slug: conductorrelay-com-faucet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-faucet-api-openapi.yml
- filename: conductorrelay-com-jobs-api-openapi.yml
  format: yaml
  label: Conductor Relay Jobs API
  slug: conductorrelay-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-jobs-api-openapi.yml
- filename: conductorrelay-com-marketplace-api-openapi.yml
  format: yaml
  label: Conductor Relay Marketplace API
  slug: conductorrelay-com-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-marketplace-api-openapi.yml
- filename: conductorrelay-com-me-api-openapi.yml
  format: yaml
  label: Conductor Relay Me API
  slug: conductorrelay-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-me-api-openapi.yml
- filename: conductorrelay-com-orders-api-openapi.yml
  format: yaml
  label: Conductor Relay Orders API
  slug: conductorrelay-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-orders-api-openapi.yml
- filename: conductorrelay-com-public-api-openapi.yml
  format: yaml
  label: Conductor Relay Public API
  slug: conductorrelay-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-public-api-openapi.yml
- filename: conductorrelay-com-sdk-requests-api-openapi.yml
  format: yaml
  label: Conductor Relay Sdk Requests API
  slug: conductorrelay-com-sdk-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-sdk-requests-api-openapi.yml
- filename: conductorrelay-com-skus-api-openapi.yml
  format: yaml
  label: Conductor Relay Skus API
  slug: conductorrelay-com-skus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-skus-api-openapi.yml
- filename: conductorrelay-com-status-api-openapi.yml
  format: yaml
  label: Conductor Relay Status API
  slug: conductorrelay-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conductorrelay-com/openapi/conductorrelay-com-status-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Conductor Relay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conductor Relay secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Conductor Relay
provider_slug: conductorrelay-com
scheme_count: 2
schemes:
- bearerFormat: cr_agent_...
  description: 'Self-serve agent registration returns a one-time cr_agent_... API key, sent as Authorization: Bearer on authenticated v1 endpoints. The same key works across REST, MCP and A2A.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/conductorrelay-com-openapi.yml
  - https://www.conductorrelay.com/agents/quickstart
  type: http
- bearerFormat: 43-character base64url wake grant
  description: Dedicated finite wake grant returned once by adapter registration. It is not a cr_agent_ key or OAuth token.
  name: wakeGrantAuth
  scheme: bearer
  sources:
  - openapi/_original/conductorrelay-com-openapi.json
  type: http
slug: conductorrelay-com-authentication
source_filename: conductorrelay-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://www.conductorrelay.com/agents/quickstart\n- https://www.conductorrelay.com/llms.txt\n- openapi/_original/conductorrelay-com-openapi.json\ndocs: https://www.conductorrelay.com/agents/quickstart\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: cr_agent_...\n  description: 'Self-serve agent registration returns a one-time cr_agent_... API key, sent as Authorization: Bearer on authenticated\n    v1 endpoints. The same key works across REST, MCP and A2A.'\n  sources:\n  - openapi/conductorrelay-com-openapi.yml\n  - https://www.conductorrelay.com/agents/quickstart\n- name: wakeGrantAuth\n  type: http\n  scheme: bearer\n  bearerFormat: 43-character base64url wake grant\n  description: Dedicated finite wake grant returned once by adapter registration. It is not a cr_agent_ key or OAuth token.\n  sources:\n  - openapi/_original/conductorrelay-com-openapi.json\nkey_lifecycle:\n\
  \  rotation: POST /api/v1/agent-keys/rotate (REST-only one-time key rotation)\n  emergency_revocation: POST /api/v1/agent-keys/revoke-current (REST-only emergency current-key revocation)\nmcp: 'MCP clients may provide the key as Authorization: Bearer ${CR_AGENT_KEY}, or apiKey configuration where supported by\n  the MCP host or gateway (llms.txt). llms.txt also refers to an OAuth connection for MCP; no OAuth scopes are documented.'\nnotes:\n- 'Send a User-Agent header: the edge rejects the default Python-urllib/3.x signature with 403 error code 1010 before authentication\n  is evaluated (quickstart).'\n"
source_yaml_url: https://artifacts.apis.io/conductorrelay-com/authentication/conductorrelay-com-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- AI Agents
- Agent Marketplace
- Governed Execution
- Agent Certification
- A2A
- MCP
- Agentic Commerce
---
