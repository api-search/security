---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentline-cloud-agent-integration-api-openapi.yml
  format: yaml
  label: AgentLine Agent Integration API
  slug: agentline-cloud-agent-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-agent-integration-api-openapi.yml
- filename: agentline-cloud-agent-recharge-api-openapi.yml
  format: yaml
  label: AgentLine Agent Recharge API
  slug: agentline-cloud-agent-recharge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-agent-recharge-api-openapi.yml
- filename: agentline-cloud-agents-api-openapi.yml
  format: yaml
  label: AgentLine Agents API
  slug: agentline-cloud-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-agents-api-openapi.yml
- filename: agentline-cloud-auth-api-openapi.yml
  format: yaml
  label: AgentLine Auth API
  slug: agentline-cloud-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-auth-api-openapi.yml
- filename: agentline-cloud-billing-api-openapi.yml
  format: yaml
  label: AgentLine Billing API
  slug: agentline-cloud-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-billing-api-openapi.yml
- filename: agentline-cloud-calls-api-openapi.yml
  format: yaml
  label: AgentLine Calls API
  slug: agentline-cloud-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-calls-api-openapi.yml
- filename: agentline-cloud-contacts-api-openapi.yml
  format: yaml
  label: AgentLine Contacts API
  slug: agentline-cloud-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-contacts-api-openapi.yml
- filename: agentline-cloud-events-api-openapi.yml
  format: yaml
  label: AgentLine Events API
  slug: agentline-cloud-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-events-api-openapi.yml
- filename: agentline-cloud-feedback-api-openapi.yml
  format: yaml
  label: AgentLine Feedback API
  slug: agentline-cloud-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-feedback-api-openapi.yml
- filename: agentline-cloud-health-api-openapi.yml
  format: yaml
  label: AgentLine Health API
  slug: agentline-cloud-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-health-api-openapi.yml
- filename: agentline-cloud-messages-api-openapi.yml
  format: yaml
  label: AgentLine Messages API
  slug: agentline-cloud-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-messages-api-openapi.yml
- filename: agentline-cloud-numbers-api-openapi.yml
  format: yaml
  label: AgentLine Numbers API
  slug: agentline-cloud-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-numbers-api-openapi.yml
- filename: agentline-cloud-usage-api-openapi.yml
  format: yaml
  label: AgentLine Usage API
  slug: agentline-cloud-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-usage-api-openapi.yml
- filename: agentline-cloud-voice-api-openapi.yml
  format: yaml
  label: AgentLine Voice API
  slug: agentline-cloud-voice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-voice-api-openapi.yml
- filename: agentline-cloud-webhooks-api-openapi.yml
  format: yaml
  label: AgentLine Webhooks API
  slug: agentline-cloud-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-webhooks-api-openapi.yml
- filename: agentline-cloud-x402-discovery-api-openapi.yml
  format: yaml
  label: AgentLine x402 Discovery API
  slug: agentline-cloud-x402-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-x402-discovery-api-openapi.yml
- filename: agentline-cloud-x402-keyless-api-openapi.yml
  format: yaml
  label: AgentLine x402 Keyless API
  slug: agentline-cloud-x402-keyless-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-x402-keyless-api-openapi.yml
auth_types: []
description: 'AgentLine uses Bearer API keys. Every authenticated request needs:'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agentline Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentLine declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AgentLine
provider_slug: agentline-cloud
scheme_count: 1
schemes:
- evidence: 'AgentLine uses **Bearer API keys**. Every authenticated request needs:'
  header: Authorization
  how_to_obtain: 'Sign‑up and sign‑in use an email one‑time‑code flow: POST /v1/auth/otp to request a code, then POST /v1/auth/verify with the code to receive an `api_key` (shown once).'
  location: header
  name: Bearer API key
  type: http-bearer
slug: agentline-cloud-authentication
source_filename: agentline-cloud-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.agentline.cloud/authentication.md
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.agentline.cloud/authentication.md\nsources:\n- https://docs.agentline.cloud/authentication.md\n- https://docs.agentline.cloud/quickstart.md\ndescription: 'AgentLine uses Bearer API keys. Every authenticated request needs:'\nschemes:\n- type: http-bearer\n  name: Bearer API key\n  evidence: 'AgentLine uses **Bearer API keys**. Every authenticated request needs:'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Sign‑up and sign‑in use an email one‑time‑code flow: POST /v1/auth/otp to request a code, then POST /v1/auth/verify with the\n    code to receive an `api_key` (shown once).'\nnote: No OAuth2, apiKey, or other authentication schemes are documented.\ndocs: https://docs.agentline.cloud/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/agentline-cloud/authentication/agentline-cloud-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Telephony
- Voice
- SMS
- Agents
---
