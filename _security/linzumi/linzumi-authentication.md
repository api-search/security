---
api_key_in: []
auth_types:
- oauth2-device-code
- oauth2-authorization-code
description: ''
kind: authentication
layout: security
method: searched
name: Linzumi Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
- authorizationCode
overview: Linzumi secures its APIs with oauth2-device-code and oauth2-authorization-code across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode and authorizationCode flow(s).
provider_name: Linzumi
provider_slug: linzumi
scheme_count: 3
schemes:
- default: true
  description: Default `linzumi connect` behaviour. Opens a browser on the runner machine and waits for an OAuth callback on localhost. Cannot work on headless machines with no browser or no loopback callback.
  flow: authorizationCode
  name: BrowserLoopbackFlow
  redirect: http://localhost (loopback callback)
  sources:
  - https://www.npmjs.com/package/@linzumi/cli
  type: oauth2
- code_expiry: 10 minutes
  description: For headless or remote runners (VPS, Windows/SSH). The runner prints an 8-character user code and a verification URL; the developer approves from a browser already signed in to Linzumi on any other machine. The runner long-polls and receives a scoped token — no browser or loopback callback needed on the runner itself.
  flow: deviceCode
  grant_delivery: long-poll
  invocation: linzumi connect --workspace <slug> --auth-mode device --api-url wss://serve.linzumi.com
  name: DeviceAuthorizationFlow
  notes: The verification URL always targets the same server passed via --api-url / --linzumi-url, defaulting to wss://serve.linzumi.com.
  sources:
  - https://www.npmjs.com/package/@linzumi/cli
  standard: RFC 8628 (OAuth 2.0 Device Authorization Grant) — shape matches; not explicitly claimed by vendor
  token_type: scoped runner token
  type: oauth2
  user_code_length: 8
  verification_url: https://serve.linzumi.com/api/v2/local-codex-runner/device
- description: Initial account creation via `npx -y @linzumi/cli@latest signup` — asks for an email address and sends a sign-in code.
  name: SignupEmailCode
  sources:
  - https://www.npmjs.com/package/@linzumi/cli
  type: email-otp
slug: linzumi-authentication
source_filename: linzumi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.npmjs.com/package/@linzumi/cli\ndocs: https://www.npmjs.com/package/@linzumi/cli\nnotes: >-\n  Derived from the published @linzumi/cli documentation rather than an OpenAPI — Linzumi publishes no\n  spec and no securitySchemes. The auth model below is what the first-party CLI documents for\n  authenticating a local runner against serve.linzumi.com. No public API-key program, no documented\n  OAuth scope surface, so `scopes/` is intentionally not created.\nsummary:\n  types:\n  - oauth2-device-code\n  - oauth2-authorization-code\n  token_transport:\n  - websocket\n  - https\n  api_key_in: []\n  oauth2_flows:\n  - deviceCode\n  - authorizationCode\nschemes:\n- name: BrowserLoopbackFlow\n  type: oauth2\n  flow: authorizationCode\n  default: true\n  description: >-\n    Default `linzumi connect` behaviour. Opens a browser on the runner machine and waits for an OAuth\n    callback on localhost. Cannot work on headless\
  \ machines with no browser or no loopback callback.\n  redirect: http://localhost (loopback callback)\n  sources:\n  - https://www.npmjs.com/package/@linzumi/cli\n- name: DeviceAuthorizationFlow\n  type: oauth2\n  flow: deviceCode\n  standard: RFC 8628 (OAuth 2.0 Device Authorization Grant) — shape matches; not explicitly claimed by vendor\n  description: >-\n    For headless or remote runners (VPS, Windows/SSH). The runner prints an 8-character user code and\n    a verification URL; the developer approves from a browser already signed in to Linzumi on any\n    other machine. The runner long-polls and receives a scoped token — no browser or loopback callback\n    needed on the runner itself.\n  invocation: linzumi connect --workspace <slug> --auth-mode device --api-url wss://serve.linzumi.com\n  verification_url: https://serve.linzumi.com/api/v2/local-codex-runner/device\n  user_code_length: 8\n  code_expiry: 10 minutes\n  grant_delivery: long-poll\n  token_type: scoped runner token\n\
  \  notes: >-\n    The verification URL always targets the same server passed via --api-url / --linzumi-url,\n    defaulting to wss://serve.linzumi.com.\n  sources:\n  - https://www.npmjs.com/package/@linzumi/cli\n- name: SignupEmailCode\n  type: email-otp\n  description: >-\n    Initial account creation via `npx -y @linzumi/cli@latest signup` — asks for an email address and\n    sends a sign-in code.\n  sources:\n  - https://www.npmjs.com/package/@linzumi/cli\nauthorization_boundaries:\n- name: Trusted folders\n  description: >-\n    Agents may only edit inside folders explicitly trusted by the developer. The trust list lives at\n    ~/.linzumi/config.json; `linzumi paths add <dir>` extends it, and the --cwd selected for\n    `linzumi connect` is trusted for that runner process.\n- name: Scoped MCP context\n  description: >-\n    The bundled local MCP server reuses the approved local-runner auth, bounding agent reads to the\n    runner's authorized message, thread, and channel context.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linzumi/refs/heads/main/authentication/linzumi-authentication.yml
summary_line: oauth2-device-code/oauth2-authorization-code · 3 schemes
tags:
- Company
- Artificial Intelligence
- Developer Tools
- Coding Agents
- Team Chat
- Collaboration
- MCP
- Command Line Interface
- Y Combinator
---
