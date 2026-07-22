---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Specific Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
overview: Specific secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and deviceCode flow(s).
provider_name: Specific
provider_slug: specific
scheme_count: 2
schemes:
- authorization_endpoint: https://api.workos.com/user_management/authorize
  evidence: dashboard.specific.dev/.well-known/openid-configuration redirects into WorkOS AuthKit (api.workos.com/user_management/authorize) with PKCE (code_challenge_method=S256).
  flow: authorizationCode
  name: WorkOS AuthKit (browser)
  pkce: true
  type: oauth2
- command: specific login --device-code
  evidence: Docs describe a device-code login flow for headless/remote agent environments; the CLI prints an authorization code the agent completes without a browser.
  flow: deviceCode
  name: Device code login
  type: oauth2
slug: specific-authentication
source_filename: specific-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.specific.dev/coding-agents\nsummary:\n  types: [oauth2]\n  identity_provider: WorkOS AuthKit\n  api_key_in: []\n  oauth2_flows: [authorizationCode, deviceCode]\nschemes:\n- name: WorkOS AuthKit (browser)\n  type: oauth2\n  flow: authorizationCode\n  authorization_endpoint: https://api.workos.com/user_management/authorize\n  pkce: true\n  evidence: >-\n    dashboard.specific.dev/.well-known/openid-configuration redirects into WorkOS AuthKit\n    (api.workos.com/user_management/authorize) with PKCE (code_challenge_method=S256).\n- name: Device code login\n  type: oauth2\n  flow: deviceCode\n  command: specific login --device-code\n  evidence: >-\n    Docs describe a device-code login flow for headless/remote agent environments; the CLI prints an\n    authorization code the agent completes without a browser.\nnotes: >-\n  Specific is account/session-authenticated through the CLI (`specific login`) backed by WorkOS\n\
  \  AuthKit OAuth; no static API keys are documented. There is no published OpenAPI declaring security\n  schemes, so this profile was searched from the docs and the live OIDC discovery redirect rather than\n  derived.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/specific/refs/heads/main/authentication/specific-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Infrastructure
- Infrastructure as Code
- Platform as a Service
- Backend as a Service
- Coding Agents
- Deployment
- PostgreSQL
- Developer Tools
- Cloud
- CLI
- MCP
---
