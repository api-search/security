---
api_key_in:
- header
api_specs:
- filename: understudy-labs-desktop-api-openapi.json
  format: json
  label: Understudy Desktop Agent API
  slug: understudy-desktop-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/understudy-labs/refs/heads/main/openapi/understudy-labs-desktop-api-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Understudy Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Understudy Labs secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Understudy Labs
provider_slug: understudy-labs
scheme_count: 5
schemes:
- description: Understudy sk_live_* key sent Anthropic-style on POST /v1/messages.
  in: header
  name: understudyKeyAnthropicStyle
  parameter: x-api-key
  sources:
  - https://docs.understudylabs.com/authentication
  type: apiKey
- description: Understudy sk_live_* key as Authorization Bearer - OpenAI-style; works on /v1/chat/completions, /v1/models, and every /admin/v1 + /customer/v1 control-plane route.
  name: understudyKeyBearer
  scheme: bearer
  sources:
  - https://docs.understudylabs.com/authentication
  - https://docs.understudylabs.com/reference/control-plane
  type: http
- description: Bring-your-own Anthropic or OpenAI provider key, forwarded upstream for that single request and never stored. Never the credential Understudy validates; rejected on routed workloads.
  in: header
  name: upstreamProviderKey
  parameter: x-understudy-upstream-key
  sources:
  - https://docs.understudylabs.com/reference/request-headers
  type: apiKey
- description: Ephemeral loopback token for the Understudy Desktop Agent API, read from the owner-only desktop capability file (~/.understudy/desktop-api.json, mode 0600). Agents should use the Understudy CLI or MCP adapter instead of handling this token directly.
  name: desktopBearer
  scheme: bearer
  sources:
  - openapi/understudy-labs-desktop-api-openapi.json
  type: http
- description: Agent-native registration flow advertised in the RFC 9728-style protected-resource metadata at /.well-known/oauth-authorization-server - register at /agent/auth, claim at /agent/auth/claim, revoke at /agent/auth/revoke; identity via verified_email assertion, credential type api_key (WorkOS agent-auth skill).
  name: agentAuthWorkOS
  scheme: bearer
  sources:
  - well-known/understudy-labs-oauth-authorization-server.json
  type: http
slug: understudy-labs-authentication
source_filename: understudy-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.understudylabs.com/authentication\ndocs: https://docs.understudylabs.com/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  notes: One credential - the Understudy sk_* key - authenticates the gateway proxy,\n    the control-plane API, and the agent CLI. Header placement depends on the API\n    shape being spoken. Keys are minted/revoked on the dashboard; plaintext is\n    shown exactly once at creation. Keys are org-scoped; captures are attributed\n    to the key id. No OAuth scopes surface is published.\nschemes:\n- name: understudyKeyAnthropicStyle\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Understudy sk_live_* key sent Anthropic-style on POST /v1/messages.\n  sources:\n  - https://docs.understudylabs.com/authentication\n- name: understudyKeyBearer\n  type: http\n  scheme: bearer\n  description: Understudy sk_live_* key as Authorization Bearer - OpenAI-style;\
  \ works\n    on /v1/chat/completions, /v1/models, and every /admin/v1 + /customer/v1\n    control-plane route.\n  sources:\n  - https://docs.understudylabs.com/authentication\n  - https://docs.understudylabs.com/reference/control-plane\n- name: upstreamProviderKey\n  type: apiKey\n  in: header\n  parameter: x-understudy-upstream-key\n  description: Bring-your-own Anthropic or OpenAI provider key, forwarded upstream\n    for that single request and never stored. Never the credential Understudy\n    validates; rejected on routed workloads.\n  sources:\n  - https://docs.understudylabs.com/reference/request-headers\n- name: desktopBearer\n  type: http\n  scheme: bearer\n  description: Ephemeral loopback token for the Understudy Desktop Agent API, read\n    from the owner-only desktop capability file (~/.understudy/desktop-api.json,\n    mode 0600). Agents should use the Understudy CLI or MCP adapter instead of\n    handling this token directly.\n  sources:\n  - openapi/understudy-labs-desktop-api-openapi.json\n\
  - name: agentAuthWorkOS\n  type: http\n  scheme: bearer\n  description: Agent-native registration flow advertised in the RFC 9728-style\n    protected-resource metadata at /.well-known/oauth-authorization-server -\n    register at /agent/auth, claim at /agent/auth/claim, revoke at\n    /agent/auth/revoke; identity via verified_email assertion, credential type\n    api_key (WorkOS agent-auth skill).\n  sources:\n  - well-known/understudy-labs-oauth-authorization-server.json\nfailure_modes:\n- status: 401\n  type: authentication_error\n  when: sk_* key missing, malformed, revoked, or unknown\n- status: 403\n  type: authorization_error\n  when: valid key used against another organization's resources\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/understudy-labs/refs/heads/main/authentication/understudy-labs-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Artificial Intelligence
- LLM Gateway
- Machine Learning
- Open Source
- Model Routing
- Evaluations
- Fine-Tuning
- AI Infrastructure
- Developer Tools
---
