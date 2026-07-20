---
api_key_in:
- header
- query
auth_types:
- apiKey
- http
- oauth2
description: Authentication profile for Digger's products. OpenComputer's REST API is API-key based with three credential types for durable agent sessions; the self-hostable OpenTaco (Digger CE) backend authenticates operators via WorkOS OIDC and integrates with source control via a GitHub App.
kind: authentication
layout: security
method: searched
name: Digger Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Digger secures its APIs with apiKey, http, and oauth2 across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Digger
provider_slug: digger
scheme_count: 6
schemes:
- in: header
  name: OrgApiKey
  notes: 'Server-side only. The v3 sessions surface also accepts the same key as an HTTP Bearer token (Authorization: Bearer $OPENCOMPUTER_API_KEY).'
  parameter: X-API-Key
  product: OpenComputer
  scope: full-account (management calls — create agents/sessions, register webhooks, manage credentials)
  source: https://docs.opencomputer.dev/api-reference/overview
  type: apiKey
- name: BearerToken
  notes: Org API key presented as Bearer on the v3 sessions API.
  product: OpenComputer (api.opencomputer.dev/v3)
  scheme: bearer
  source: https://docs.opencomputer.dev/agent-sessions/authentication
  type: http
- browser_safe: true
  lifetime: short-lived, session-scoped (ttlSeconds, e.g. 3600)
  minted_via: POST /v3/sessions or POST /v3/sessions/{id}/client-tokens
  name: ClientToken
  notes: Session-scoped token safe to hand to a front-end. Can stream and steer ONE session and nothing else. Never ship the org API key to a browser.
  product: OpenComputer
  scheme: bearer
  source: https://docs.opencomputer.dev/agent-sessions/authentication
  token_scopes:
  - read
  - steer
  type: http
- in: query
  name: WebSocketQueryKey
  notes: WebSocket exec endpoints accept the API key via query parameter.
  parameter: api_key
  product: OpenComputer
  source: https://docs.opencomputer.dev/api-reference/overview
  type: apiKey
- name: WorkOS-OIDC
  notes: Operator sign-in for the self-hosted OpenTaco dashboard is configured via WorkOS.
  product: OpenTaco (Digger CE self-host backend)
  source: https://docs.opentaco.dev/self-hosting/workos-setup
  type: openIdConnect
- flow: authorizationCode
  name: GitHubApp
  notes: PR automation and source-control integration run through an installed GitHub App.
  product: OpenTaco (Digger CE)
  source: https://docs.opentaco.dev/onboarding/github-app-setup
  type: oauth2
slug: digger-authentication
source_filename: digger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.opencomputer.dev/agent-sessions/authentication\ndocs: https://docs.opencomputer.dev/agent-sessions/authentication\ndescription: >-\n  Authentication profile for Digger's products. OpenComputer's REST API is\n  API-key based with three credential types for durable agent sessions; the\n  self-hostable OpenTaco (Digger CE) backend authenticates operators via WorkOS\n  OIDC and integrates with source control via a GitHub App.\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header, query]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: OrgApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  product: OpenComputer\n  scope: full-account (management calls — create agents/sessions, register webhooks, manage credentials)\n  notes: >-\n    Server-side only. The v3 sessions surface also accepts the same key as an\n    HTTP Bearer token (Authorization: Bearer $OPENCOMPUTER_API_KEY).\n  source:\
  \ https://docs.opencomputer.dev/api-reference/overview\n- name: BearerToken\n  type: http\n  scheme: bearer\n  product: OpenComputer (api.opencomputer.dev/v3)\n  notes: Org API key presented as Bearer on the v3 sessions API.\n  source: https://docs.opencomputer.dev/agent-sessions/authentication\n- name: ClientToken\n  type: http\n  scheme: bearer\n  product: OpenComputer\n  token_scopes: [read, steer]\n  lifetime: short-lived, session-scoped (ttlSeconds, e.g. 3600)\n  browser_safe: true\n  minted_via: POST /v3/sessions or POST /v3/sessions/{id}/client-tokens\n  notes: >-\n    Session-scoped token safe to hand to a front-end. Can stream and steer ONE\n    session and nothing else. Never ship the org API key to a browser.\n  source: https://docs.opencomputer.dev/agent-sessions/authentication\n- name: WebSocketQueryKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  product: OpenComputer\n  notes: WebSocket exec endpoints accept the API key via query parameter.\n  source: https://docs.opencomputer.dev/api-reference/overview\n\
  - name: WorkOS-OIDC\n  type: openIdConnect\n  product: OpenTaco (Digger CE self-host backend)\n  notes: Operator sign-in for the self-hosted OpenTaco dashboard is configured via WorkOS.\n  source: https://docs.opentaco.dev/self-hosting/workos-setup\n- name: GitHubApp\n  type: oauth2\n  flow: authorizationCode\n  product: OpenTaco (Digger CE)\n  notes: PR automation and source-control integration run through an installed GitHub App.\n  source: https://docs.opentaco.dev/onboarding/github-app-setup\nbyo_credentials:\n  bring_your_own_model_keys: true\n  notes: OpenComputer agent sessions support bring-your-own model provider keys.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digger/refs/heads/main/authentication/digger-authentication.yml
summary_line: apiKey/http/oauth2 · 6 schemes
tags:
- Company
- AI Agents
- Cloud Sandbox
- Compute
- Infrastructure as Code
- Terraform
- OpenTofu
- Developer Tools
- Webhooks
- Open Source
- SDKs
- CLI
---
