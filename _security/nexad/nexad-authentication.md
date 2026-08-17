---
api_key_in:
- sdk-config
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nexad Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
overview: Nexad secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode flow(s).
provider_name: Nexad
provider_slug: nexad
scheme_count: 2
schemes:
- credentials:
  - App ID
  - Publisher ID
  in: sdk-config
  name: nexad-android-sdk
  product: Nexad Android Ads SDK
  provisioning: Credentials are issued after submitting the Nexad contact form; the team returns a unique App ID and Publisher ID passed to NexadSDK.initialize(). There is no self-serve key issuance for the SDK.
  source: https://docs.nex.ad/docs/android/getting-started
  type: apiKey
- authorization:
    detail: Least-privilege is enforced at EXECUTION time rather than at token-issue time. 124 of 281 published actions carry requires_review=true and create a pending review that a human must approve before the write executes. This is an unusual and, for an agent-facing API, a defensible substitute for scopes — but it does mean a leaked token grants full read access to every connected ad and analytics account immediately.
    mechanism: human review gate
    see: agentic-access/nexad-agentic-access.yml
  detail: The Soku CLI authenticates via an OAuth device-login flow (`soku auth login`), returning a verification_uri and a user_code and resumable with `--device-code <device_code>`. Direct calls to api.soku.ai/v1, api.soku.ai/api/cli and api.soku.ai/mcp return HTTP 401 without a token. Third-party provider credentials are injected SERVER-SIDE via `soku egress` rather than handled by the user.
  endpoint: https://api.soku.ai
  flow: deviceCode
  name: soku-nexstudio-api
  observed_challenges:
    checked: '2026-08-13'
    probes:
    - body: '{"success":false,"data":null,"error":{"code":"unauthorized","message":"Invalid or expired token","details":null},"meta":null}'
      status: 401
      url: https://api.soku.ai/v1
    - body: '{"error":"missing_bearer","message":"missing_bearer"}'
      status: 401
      url: https://api.soku.ai/api/cli/capabilities
    - note: tools/list JSON-RPC POST; no WWW-Authenticate header returned
      status: 401
      url: https://api.soku.ai/mcp
  product: Soku (NexStudio) API
  rotation:
    guidance: Published in SECURITY.md — rotate immediately if a token may have been exposed.
    procedure: soku auth logout then soku auth login
  scopes:
    published: false
    statement: 'Quoted from the provider''s own reference doc: "A default `soku auth login` reaches the entire CLI surface — there is no resource model to grant or check." A token is therefore all-or-nothing across 281 actions. No scopes/ artifact is emitted for this provider because there is no scope surface to capture.'
  source: https://soku.ai/cli/skill.md
  standard: OAuth 2.0 Device Authorization Grant (RFC 8628)
  token_storage:
    bypass: SOKU_NO_KEYCHAIN=1 (recommended for shell/container agents to avoid an indefinite keychain/D-Bus wait)
    env_injection: SOKU_TOKEN (the provider's preferred path for CI and headless agents)
    fallback: file-backed store at ~/.soku/credentials.json, mode 0600
    primary: OS keychain via keytar (optional dependency)
  token_type: Bearer
  type: oauth2
slug: nexad-authentication
source_filename: nexad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource:\n  - https://docs.nex.ad/docs/android/getting-started\n  - https://soku.ai/cli/skill.md\n  - https://raw.githubusercontent.com/About-Intelligence/soku-cli/main/skills/soku/references/auth-workspace.md\n  - https://raw.githubusercontent.com/About-Intelligence/soku-cli/main/skills/soku/references/egress-security.md\n  - https://raw.githubusercontent.com/About-Intelligence/soku-cli/main/SECURITY.md\n  - https://api.soku.ai/api/cli/capabilities\nnotes: >-\n  Nexad has no published OpenAPI, so this profile is searched from provider docs\n  and live probes rather than derived from securitySchemes. Two distinct products\n  with two distinct auth models. Upgraded 2026-08-13 with the token-storage,\n  rotation and third-party credential model published in the company's own repo,\n  and with the observed 401 challenge shapes.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [sdk-config]\n  oauth2_flows: [deviceCode]\n  scopes_published:\
  \ false\n  authorization_model: human-review-gate\nschemes:\n  - name: nexad-android-sdk\n    product: Nexad Android Ads SDK\n    type: apiKey\n    credentials:\n      - App ID\n      - Publisher ID\n    in: sdk-config\n    provisioning: >-\n      Credentials are issued after submitting the Nexad contact form; the team\n      returns a unique App ID and Publisher ID passed to NexadSDK.initialize().\n      There is no self-serve key issuance for the SDK.\n    source: https://docs.nex.ad/docs/android/getting-started\n  - name: soku-nexstudio-api\n    product: Soku (NexStudio) API\n    type: oauth2\n    flow: deviceCode\n    standard: OAuth 2.0 Device Authorization Grant (RFC 8628)\n    endpoint: https://api.soku.ai\n    token_type: Bearer\n    detail: >-\n      The Soku CLI authenticates via an OAuth device-login flow (`soku auth\n      login`), returning a verification_uri and a user_code and resumable with\n      `--device-code <device_code>`. Direct calls to api.soku.ai/v1,\n      api.soku.ai/api/cli\
  \ and api.soku.ai/mcp return HTTP 401 without a token.\n      Third-party provider credentials are injected SERVER-SIDE via `soku egress`\n      rather than handled by the user.\n    source: https://soku.ai/cli/skill.md\n    token_storage:\n      primary: OS keychain via keytar (optional dependency)\n      fallback: file-backed store at ~/.soku/credentials.json, mode 0600\n      bypass: SOKU_NO_KEYCHAIN=1 (recommended for shell/container agents to avoid an indefinite keychain/D-Bus wait)\n      env_injection: SOKU_TOKEN (the provider's preferred path for CI and headless agents)\n    rotation:\n      procedure: soku auth logout then soku auth login\n      guidance: Published in SECURITY.md — rotate immediately if a token may have been exposed.\n    scopes:\n      published: false\n      statement: >-\n        Quoted from the provider's own reference doc: \"A default `soku auth login`\n        reaches the entire CLI surface — there is no resource model to grant or\n        check.\" A token\
  \ is therefore all-or-nothing across 281 actions. No\n        scopes/ artifact is emitted for this provider because there is no scope\n        surface to capture.\n    authorization:\n      mechanism: human review gate\n      detail: >-\n        Least-privilege is enforced at EXECUTION time rather than at token-issue\n        time. 124 of 281 published actions carry requires_review=true and create a\n        pending review that a human must approve before the write executes. This is\n        an unusual and, for an agent-facing API, a defensible substitute for\n        scopes — but it does mean a leaked token grants full read access to every\n        connected ad and analytics account immediately.\n      see: agentic-access/nexad-agentic-access.yml\n    observed_challenges:\n      checked: '2026-08-13'\n      probes:\n        - {url: 'https://api.soku.ai/v1', status: 401, body: '{\"success\":false,\"data\":null,\"error\":{\"code\":\"unauthorized\",\"message\":\"Invalid or expired token\"\
  ,\"details\":null},\"meta\":null}'}\n        - {url: 'https://api.soku.ai/api/cli/capabilities', status: 401, body: '{\"error\":\"missing_bearer\",\"message\":\"missing_bearer\"}'}\n        - {url: 'https://api.soku.ai/mcp', status: 401, note: 'tools/list JSON-RPC POST; no WWW-Authenticate header returned'}\nthird_party_credentials:\n  model: server-side injection\n  detail: >-\n    For covered third-party APIs the caller never holds the key. `soku egress --\n    curl ...` strips empty placeholder auth and Soku injects the real credential\n    server-side. `soku egress providers` lists covered hosts. The provider\n    explicitly instructs agents NOT to preflight or guard on a local key env var.\n  source: https://raw.githubusercontent.com/About-Intelligence/soku-cli/main/skills/soku/references/egress-security.md\ndiscovery_gaps:\n  - {document: /.well-known/openid-configuration, status: 404-or-401, impact: No OIDC discovery.}\n  - {document: /.well-known/oauth-authorization-server, status:\
  \ 404-or-401, impact: 'No RFC 8414 metadata; device/token endpoints are undiscoverable outside the CLI.'}\n  - {document: /.well-known/oauth-protected-resource, status: 401, impact: 'No RFC 9728 metadata, so an MCP client cannot discover how to authorize against /mcp.'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexad/refs/heads/main/authentication/nexad-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Advertising
- Marketing
- Marketing Automation
- Contextual Advertising
- Mobile SDK
- Agent
---
