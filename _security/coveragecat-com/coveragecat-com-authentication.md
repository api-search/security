---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coveragecat-com-agent-api-openapi.yml
  format: yaml
  label: Coverage Cat Agent API
  slug: coveragecat-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coveragecat-com/openapi/coveragecat-com-agent-api-openapi.yml
- filename: coveragecat-com-consumer-api-openapi.yml
  format: yaml
  label: Coverage Cat Consumer API
  slug: coveragecat-com-consumer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coveragecat-com/openapi/coveragecat-com-consumer-api-openapi.yml
- filename: coveragecat-com-intake-api-openapi.yml
  format: yaml
  label: Coverage Cat Intake API
  slug: coveragecat-com-intake-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coveragecat-com/openapi/coveragecat-com-intake-api-openapi.yml
- filename: coveragecat-com-tools-api-openapi.yml
  format: yaml
  label: Coverage Cat Tools API
  slug: coveragecat-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coveragecat-com/openapi/coveragecat-com-tools-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Coverage Cat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coverage Cat secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Coverage Cat
provider_slug: coveragecat-com
scheme_count: 3
schemes:
- description: 'Operator-issued bearer key (shown in docs with the ccop_ prefix, e.g. "Authorization: Bearer ccop_..."). Issued via an emailed OTP flow (POST /api/agent/key/request then POST /api/agent/key/confirm) and rotated with POST /api/agent/key/rotate, which invalidates the old token. Use the operator or integrator email, never the end-customer email.'
  name: agent_api_key
  required_for:
  - POST /api/agent/umbrella/draft
  - POST /api/agent/umbrella/quotes
  - POST /api/agent/umbrella/select
  - POST /api/agent/umbrella/bind
  - POST /api/agent/umbrella/status
  - POST /api/agent/umbrella/attach
  - POST /api/agent/homeowners/quotes
  - GET /api/agent/homeowners/dashboard
  - POST /api/agent/homeowners/dashboard/session
  - POST /api/agent/homeowners/fix-issues-email
  scheme: bearer
  sources:
  - openapi/coveragecat-com-agent-openapi.yml
  - openapi/coveragecat-com-consumer-openapi.yml
  - https://www.coveragecat.com/developers/auth
  type: http
- description: Short-lived bearer token returned by consumer-prefill and rotated by each successful direct follow-up response (consumer /api/intake/{uid}/* flow).
  name: intake_access_token
  scheme: bearer
  sources:
  - openapi/coveragecat-com-agent-openapi.yml
  - openapi/coveragecat-com-consumer-openapi.yml
  type: http
- description: Documented (not declared in the OpenAPI) primary path — a user-claimed OAuth flow that returns a short-lived id-jag identity assertion and then exchanges it for an access_token. Docs list /agent/identity, /agent/identity/claim, /oauth2/token and /oauth2/revoke, plus /.well-known/oauth-protected-resource and /.well-known/oauth-authorization-server discovery. Compatibility endpoints /agent/auth, /agent/auth/claim and /agent/auth/revoke support direct OTP claims for a short-lived access_token or a longer-lived api_key. Not called by this pipeline.
  name: agent_identity_oauth
  sources:
  - https://www.coveragecat.com/developers/auth
  type: oauth2
slug: coveragecat-com-authentication
source_filename: coveragecat-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.coveragecat.com/developers/auth\ndocs: https://www.coveragecat.com/developers/auth\nderived_from:\n- openapi/coveragecat-com-agent-openapi.yml\n- openapi/coveragecat-com-consumer-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: agent_api_key\n  type: http\n  scheme: bearer\n  description: 'Operator-issued bearer key (shown in docs with the ccop_ prefix, e.g. \"Authorization: Bearer ccop_...\"). Issued via an emailed OTP flow (POST /api/agent/key/request then POST /api/agent/key/confirm) and rotated with POST /api/agent/key/rotate, which invalidates the old token. Use the operator or integrator email, never the end-customer email.'\n  required_for:\n  - POST /api/agent/umbrella/draft\n  - POST /api/agent/umbrella/quotes\n  - POST /api/agent/umbrella/select\n  - POST /api/agent/umbrella/bind\n  - POST /api/agent/umbrella/status\n  - POST /api/agent/umbrella/attach\n  - POST /api/agent/homeowners/quotes\n\
  \  - GET /api/agent/homeowners/dashboard\n  - POST /api/agent/homeowners/dashboard/session\n  - POST /api/agent/homeowners/fix-issues-email\n  sources:\n  - openapi/coveragecat-com-agent-openapi.yml\n  - openapi/coveragecat-com-consumer-openapi.yml\n  - https://www.coveragecat.com/developers/auth\n- name: intake_access_token\n  type: http\n  scheme: bearer\n  description: 'Short-lived bearer token returned by consumer-prefill and rotated by each successful direct follow-up response (consumer /api/intake/{uid}/* flow).'\n  sources:\n  - openapi/coveragecat-com-agent-openapi.yml\n  - openapi/coveragecat-com-consumer-openapi.yml\n- name: agent_identity_oauth\n  type: oauth2\n  description: 'Documented (not declared in the OpenAPI) primary path — a user-claimed OAuth flow that returns a short-lived id-jag identity assertion and then exchanges it for an access_token. Docs list /agent/identity, /agent/identity/claim, /oauth2/token and /oauth2/revoke, plus /.well-known/oauth-protected-resource\
  \ and /.well-known/oauth-authorization-server discovery. Compatibility endpoints /agent/auth, /agent/auth/claim and /agent/auth/revoke support direct OTP claims for a short-lived access_token or a longer-lived api_key. Not called by this pipeline.'\n  sources:\n  - https://www.coveragecat.com/developers/auth\npublic_surface: Consumer prefill (/api/consumer/umbrella/prefill, /api/consumer/homeowners/prefill), coarse status polling, discovery (/api/agent, /api/consumer), OpenAPI documents and read-only calculators require no operator key.\nguardrails:\n- Store the issued key in a server-side secret manager.\n- Do not embed the key in browser code or customer-visible prompts.\n- Do not use shared environment keys where Coverage Cat explicitly requires operator-issued keys.\n"
source_yaml_url: https://artifacts.apis.io/coveragecat-com/authentication/coveragecat-com-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Insurance
- Insurance Broker
- Home Insurance
- Umbrella Insurance
- Auto Insurance
- AI Agents
- MCP
---
