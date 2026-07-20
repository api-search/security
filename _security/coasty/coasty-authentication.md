---
api_key_in:
- header
api_specs:
- filename: coasty-openapi-original.json
  format: json
  label: Coasty Public API
  slug: coasty-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coasty/refs/heads/main/openapi/coasty-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Coasty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coasty secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Coasty
provider_slug: coasty
scheme_count: 4
schemes:
- description: 'Coasty API key. Live: `sk-coasty-live-...`. Sandbox: `sk-coasty-test-...`.'
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/coasty-openapi-original.json
  type: apiKey
- bearerFormat: Coasty API key (sk-coasty-{live,test}-...)
  description: Equivalent to X-API-Key. Use whichever your client supports.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/coasty-openapi-original.json
  type: http
- description: 'HMAC-SHA256 credential for external schedule webhooks: t=<unix_ts>,v1=<hex_digest>.'
  in: header
  name: webhookHmac
  parameter: Coasty-Signature
  sources:
  - openapi/coasty-openapi-original.json
  type: apiKey
- description: Compatibility alias for the Coasty-Signature HMAC credential.
  in: header
  name: webhookHmacLegacy
  parameter: X-Coasty-Signature
  sources:
  - openapi/coasty-openapi-original.json
  type: apiKey
slug: coasty-authentication
source_filename: coasty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/coasty-openapi-original.json\ndocs: https://coasty.ai/docs\ndiscovery: https://coasty.ai/api/discovery\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  key_header: X-API-Key\n  bearer_equivalent: true\n  live_key_prefix: sk-coasty-live-\n  sandbox_key_prefix: sk-coasty-test-\n  sandbox_free: true\n  key_management: Keys are minted/revoked via POST /v1/keys, GET /v1/keys, DELETE /v1/keys/{key_id}; each key is scoped.\n  scopes:\n  - predict\n  - ground\n  - parse\n  - session\n  - keys\n  - usage\n  - machines:read\n  - machines:write\n  - actions:exec\n  - terminal:exec\n  - files:read\n  - files:write\n  - browser:execute\n  - snapshots:write\n  - connection:read\n  - schedules:read\n  - schedules:write\n  - triggers:write\n  - runs:read\n  - runs:write\n  - workflows:read\n  - workflows:write\n  - llm_keys\n  byok:\n    description: Bring-your-own-model — run every LLM call on your own Anthropic/OpenAI\
  \ key.\n    request_headers:\n    - X-LLM-Provider\n    - X-LLM-Api-Key\n    - X-LLM-Model\n    stored_key_endpoint: PUT /v1/llm/keys/{provider}\n    at_rest: AES-256-GCM encrypted; only a sha256-prefix fingerprint is echoed.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'Coasty API key. Live: `sk-coasty-live-...`. Sandbox: `sk-coasty-test-...`.'\n  sources:\n  - openapi/coasty-openapi-original.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Coasty API key (sk-coasty-{live,test}-...)\n  description: Equivalent to X-API-Key. Use whichever your client supports.\n  sources:\n  - openapi/coasty-openapi-original.json\n- name: webhookHmac\n  type: apiKey\n  in: header\n  parameter: Coasty-Signature\n  description: 'HMAC-SHA256 credential for external schedule webhooks: t=<unix_ts>,v1=<hex_digest>.'\n  sources:\n  - openapi/coasty-openapi-original.json\n- name: webhookHmacLegacy\n  type: apiKey\n  in: header\n  parameter:\
  \ X-Coasty-Signature\n  description: Compatibility alias for the Coasty-Signature HMAC credential.\n  sources:\n  - openapi/coasty-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coasty/refs/heads/main/authentication/coasty-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Computer Use
- AI Agents
- Automation
- RPA
- Desktop Automation
- Browser Automation
- MCP
- Virtual Machines
- Developer Tools
---
