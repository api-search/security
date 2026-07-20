---
api_key_in: []
api_specs:
- filename: contextdev-openapi.yml
  format: yaml
  label: Context API
  slug: context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Contextdev Authentication
name_suffix: Authentication
oauth_flows:
- jwt-bearer
- agent-auth-claim
overview: Context.dev secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the jwt-bearer and agent-auth-claim flow(s).
provider_name: Context.dev
provider_slug: contextdev
scheme_count: 2
schemes:
- description: Static API key issued from the dashboard (prefix ctxt_secret_), sent as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/contextdev-openapi.yml
  type: http
- authorization_server: https://www.context.dev
  description: WorkOS-style agentic registration (service_auth). Agents discover the authorization server, register at /agent/identity, deliver a claim code to the user, then poll /oauth2/token. Scopes api.read + api.write.
  grant_types:
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:workos:agent-auth:grant-type:claim
  name: AgentAuth
  revocation_endpoint: https://www.context.dev/oauth2/revoke
  scopes:
  - api.read
  - api.write
  sources:
  - well-known/contextdev-oauth-authorization-server.json
  - https://www.context.dev/auth.md
  token_endpoint: https://www.context.dev/oauth2/token
  type: oauth2
slug: contextdev-authentication
source_filename: contextdev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/contextdev-openapi.yml\nmethod_note: >-\n  Derived bearerAuth from the OpenAPI, upgraded with the documented auth model\n  from https://www.context.dev/auth.md and the OAuth2 agent-auth metadata at\n  /.well-known/oauth-authorization-server.\ndocs: https://www.context.dev/auth.md\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_prefix: ctxt_secret_\n  oauth2_flows:\n  - jwt-bearer\n  - agent-auth-claim\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Static API key issued from the dashboard (prefix ctxt_secret_), sent as a\n    Bearer token in the Authorization header.\n  sources:\n  - openapi/contextdev-openapi.yml\n- name: AgentAuth\n  type: oauth2\n  description: >-\n    WorkOS-style agentic registration (service_auth). Agents discover the\n    authorization server, register at /agent/identity, deliver a claim code to\n    the user, then poll /oauth2/token. Scopes api.read\
  \ + api.write.\n  authorization_server: https://www.context.dev\n  token_endpoint: https://www.context.dev/oauth2/token\n  revocation_endpoint: https://www.context.dev/oauth2/revoke\n  scopes:\n  - api.read\n  - api.write\n  grant_types:\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:workos:agent-auth:grant-type:claim\n  sources:\n  - well-known/contextdev-oauth-authorization-server.json\n  - https://www.context.dev/auth.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/authentication/contextdev-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Web Scraping
- Brand Intelligence
- Data Enrichment
- AI Agents
- Web Data
- Classification
- Website Monitoring
- Company Data
- Developer Tools
- APIs
---
