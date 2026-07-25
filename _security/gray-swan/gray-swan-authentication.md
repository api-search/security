---
api_key_in: []
api_specs:
- filename: gray-swan-activity-api-openapi.yml
  format: yaml
  label: Gray Swan Activity API
  slug: gray-swan-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gray-swan/refs/heads/main/openapi/gray-swan-activity-api-openapi.yml
- filename: gray-swan-cygnal-api-openapi.yml
  format: yaml
  label: Gray Swan Cygnal API
  slug: gray-swan-cygnal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gray-swan/refs/heads/main/openapi/gray-swan-cygnal-api-openapi.yml
- filename: gray-swan-policies-api-openapi.yml
  format: yaml
  label: Gray Swan Policies API
  slug: gray-swan-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gray-swan/refs/heads/main/openapi/gray-swan-policies-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Gray Swan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gray Swan declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Gray Swan
provider_slug: gray-swan
scheme_count: 1
schemes:
- description: First-party API key issued from the Gray Swan platform (https://platform.grayswan.ai). Sent on every request.
  docs: https://docs.grayswan.ai/cygnal/creating-completions
  id: grayswan-api-key
  in: header
  key_provisioning: https://platform.grayswan.ai
  name: grayswan-api-key
  type: apiKey
slug: gray-swan-authentication
source_filename: gray-swan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.grayswan.ai/cygnal/creating-completions\napi: Cygnal\nsummary: >-\n  The Gray Swan AI (Cygnal) API authenticates every request with a first-party\n  API key sent in the custom `grayswan-api-key` request header. Keys are minted\n  in the Gray Swan platform. Cygnal proxy requests additionally require an\n  explicit policy selector header (`policy-id` or `agent-id`) — there is no\n  default policy. The published OpenAPI does not declare `securitySchemes`; the\n  scheme below is captured from the provider's authentication documentation.\nschemes:\n  - id: grayswan-api-key\n    type: apiKey\n    in: header\n    name: grayswan-api-key\n    description: >-\n      First-party API key issued from the Gray Swan platform\n      (https://platform.grayswan.ai). Sent on every request.\n    docs: https://docs.grayswan.ai/cygnal/creating-completions\n    key_provisioning: https://platform.grayswan.ai\nrequired_companion_headers:\n\
  \  - name: policy-id\n    required: conditional\n    description: >-\n      Identifier of the Cygnal policy to enforce on this request. Required on\n      /cygnal/* proxy endpoints unless an agent-id is supplied. Missing both\n      returns `400 No policy specified` — Cygnal never applies a default policy.\n  - name: agent-id\n    required: conditional\n    description: >-\n      Identifier of an agent that has an associated policy; an alternative to\n      policy-id for selecting the enforced policy.\nnotes:\n  - No OAuth/OIDC scopes surface — key-auth only, so no scopes/ artifact.\n  - Platform login/waitlist is brokered by Stytch (and Okta for enterprise SSO).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gray-swan/refs/heads/main/authentication/gray-swan-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Ai
- AI Security
- LLM Security
- Guardrails
- Red Teaming
- AI Governance
- Prompt Injection
- Model Safety
- API Security
---
