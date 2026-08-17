---
api_key_in:
- header
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Revnu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Revnu secures its APIs with http and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Revnu
provider_slug: revnu
scheme_count: 4
schemes:
- audience: operator
  header: Authorization
  issued_at: Revnu dashboard -> CLI -> "API Keys & MCP"
  key_prefixes:
  - rev_cli_
  - rev_
  name: agentApiKey
  scheme: bearer
  source: https://auth.revnu.app/.well-known/mcp/server-card.json
  type: http
  used_by:
  - https://auth.revnu.app/api/mcp
  - /api/agent/*
- audience: operator
  endpoints:
  - POST /api/cli/device/code
  - POST /api/cli/device/poll
  grant: device-code
  header: Authorization
  name: cliDeviceToken
  poll_states:
  - approved
  - denied
  - expired
  - used
  - invalid
  - pending
  scheme: bearer
  source: npm @revnu/cli 0.1.0
  standard_alignment: device-code shaped, but not RFC 8628 — the endpoints, the field names (userCode/deviceCode/verificationUrl/expiresAt) and the poll semantics are Revnu's own, and there is no authorization-server metadata document
  storage: ~/.revnu/credentials (0600)
  type: http
- audience: end user (browser)
  env_vars:
  - NEXT_PUBLIC_REVNU_KEY
  - VITE_REVNU_KEY
  - REVNU_KEY
  in: header
  key_prefix: rev_pub_
  name: revnuPublishableKey
  name_: X-Revnu-Key
  note: publishable, safe to ship in a client bundle; identifies the store
  source: https://auth.revnu.app/docs/auth-sdk
  type: apiKey
  used_by: https://auth.revnu.app/api/auth/revnu/*
- algorithm: RS256
  audience: end user
  bearerFormat: JWT
  claims:
  - sub
  - email
  - name
  - iat
  - exp
  - products[] (productId, status, cancelAtPeriodEnd, currentPeriodEnd)
  cookie: revnu_access_token
  issuer: revnu-auth
  name: revnuSessionJWT
  refresh: POST /api/auth/revnu/refresh (refresh token in an http-only cookie)
  scheme: bearer
  source: npm @revnu/auth 1.1.0 dist/core
  type: http
  verification: asymmetric, public key embedded in @revnu/auth — no secret to configure
slug: revnu-authentication
source_filename: revnu-authentication.yml
source_heading: Authentication Profile
source_url: https://auth.revnu.app/docs/auth-sdk
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://auth.revnu.app/docs/auth-sdk\ndocs: https://auth.revnu.app/docs/auth-sdk\nsources:\n- https://auth.revnu.app/docs/auth-sdk\n- https://auth.revnu.app/docs/mcp\n- https://auth.revnu.app/docs/cli\n- https://auth.revnu.app/.well-known/mcp/server-card.json\n- npm @revnu/auth 1.1.0 README + dist\nnote: >-\n  Revnu publishes no OpenAPI, so this profile is read from the provider's own\n  docs and first-party packages and confirmed by live probes. There is no OIDC\n  or OAuth 2.0 discovery document on any Revnu host\n  (/.well-known/openid-configuration and /.well-known/oauth-authorization-server\n  both 404), so `scopes/` is deliberately absent — Revnu is a key/JWT provider,\n  not a scoped-OAuth one.\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  audiences:\n  - operator (store owner, via CLI/MCP)\n  - end user (a store's buyer, via the Auth SDK)\nschemes:\n- name: agentApiKey\n\
  \  type: http\n  scheme: bearer\n  audience: operator\n  header: Authorization\n  key_prefixes:\n  - rev_cli_\n  - rev_\n  issued_at: Revnu dashboard -> CLI -> \"API Keys & MCP\"\n  used_by:\n  - https://auth.revnu.app/api/mcp\n  - /api/agent/*\n  source: https://auth.revnu.app/.well-known/mcp/server-card.json\n- name: cliDeviceToken\n  type: http\n  scheme: bearer\n  audience: operator\n  header: Authorization\n  grant: device-code\n  endpoints:\n  - POST /api/cli/device/code\n  - POST /api/cli/device/poll\n  poll_states:\n  - approved\n  - denied\n  - expired\n  - used\n  - invalid\n  - pending\n  storage: ~/.revnu/credentials (0600)\n  standard_alignment: device-code shaped, but not RFC 8628 — the endpoints, the field\n    names (userCode/deviceCode/verificationUrl/expiresAt) and the poll semantics are\n    Revnu's own, and there is no authorization-server metadata document\n  source: npm @revnu/cli 0.1.0\n- name: revnuPublishableKey\n  type: apiKey\n  in: header\n  name_: X-Revnu-Key\n\
  \  audience: end user (browser)\n  key_prefix: rev_pub_\n  env_vars:\n  - NEXT_PUBLIC_REVNU_KEY\n  - VITE_REVNU_KEY\n  - REVNU_KEY\n  used_by: https://auth.revnu.app/api/auth/revnu/*\n  note: publishable, safe to ship in a client bundle; identifies the store\n  source: https://auth.revnu.app/docs/auth-sdk\n- name: revnuSessionJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  audience: end user\n  algorithm: RS256\n  issuer: revnu-auth\n  verification: asymmetric, public key embedded in @revnu/auth — no secret to configure\n  cookie: revnu_access_token\n  claims:\n  - sub\n  - email\n  - name\n  - iat\n  - exp\n  - products[] (productId, status, cancelAtPeriodEnd, currentPeriodEnd)\n  refresh: POST /api/auth/revnu/refresh (refresh token in an http-only cookie)\n  source: npm @revnu/auth 1.1.0 dist/core\nmodel:\n  end_user: >-\n    Purchase-first. Buying a product creates the account; a setup-link email lets\n    the buyer set a password. There is no separate sign-up flow. Product\n\
  \    entitlement is embedded in the JWT, so access checks need no webhook and no\n    call back to Revnu.\n  operator: >-\n    Dashboard-issued bearer API key for MCP and the /api/agent REST surface, or a\n    browser-approved device-code token for the CLI.\nendpoints:\n  auth_base: https://auth.revnu.app\n  paths:\n  - POST /api/auth/revnu/sign-in\n  - POST /api/auth/revnu/sign-out\n  - POST /api/auth/revnu/refresh\n  - GET /api/auth/revnu/store-info\n  - POST /api/auth/revnu/forgot-password\n  - POST /api/auth/revnu/reset-password\n  - POST /api/auth/revnu/setup-password\n  - POST /api/auth/revnu/request-setup-link\nx-evidence:\n- url: https://auth.revnu.app/api/auth/revnu/sign-in\n  method: POST (no key)\n  status: 401\n  body: '{\"error\":\"Missing X-Revnu-Key header\"}'\n- url: https://auth.revnu.app/api/auth/revnu/store-info\n  method: GET (bad key)\n  status: 401\n  body: '{\"error\":\"Invalid public key\"}'\n- url: https://auth.revnu.app/api/agent/context\n  method: GET (no header)\n\
  \  status: 401\n  body: '{\"error\":\"Unauthorized\",\"message\":\"Invalid or expired CLI token. Run `npx @revnu/setup\n    auth login` to re-authenticate.\"}'\n- url: https://auth.revnu.app/.well-known/openid-configuration\n  status: 404\n- url: https://auth.revnu.app/.well-known/oauth-authorization-server\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revnu/refs/heads/main/authentication/revnu-authentication.yml
summary_line: http/apiKey · 4 schemes
tags:
- Company
- Growth Automation
- Marketing
- Artificial Intelligence
- SaaS
- Startups
- Lead Generation
- SEO
- MCP
- Agents
- Commerce
- A/B Testing
---
