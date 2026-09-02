---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Weaveapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: WeaveAPI - OpenAI-compatible AI API Gateway secures its APIs with apiKey across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WeaveAPI - OpenAI-compatible AI API Gateway
provider_slug: weaveapi
scheme_count: 0
schemes: []
slug: weaveapi-authentication
source_filename: weaveapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: https://weaveapi.dev/docs/\ndocs: https://weaveapi.dev/docs/\n\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  scheme: bearer\n  oauth2_flows: []\n  scopes_supported: false\n  note: >-\n    The WeaveAPI API itself has exactly one authentication mechanism: a bearer API key in the\n    Authorization header. There is no OAuth on the API surface, no scopes, no per-key permissions\n    documented, and no key-prefix convention published. The OAuth/OIDC/passkey machinery below belongs\n    to the hosted CONSOLE (human login), not to the API — the two are recorded separately because\n    conflating them would credit WeaveAPI with an API authorization model it does not have.\n\napi_authentication:\n  schemes:\n    - name: bearerAuth\n      type: http\n      scheme: bearer\n      in: header\n      parameter_name: Authorization\n      format: 'Authorization: Bearer YOUR_WEAVEAPI_KEY'\n      applies_to: All /v1 routes\n      source:\
  \ https://weaveapi.dev/docs/\n      issued_via: Console → Token Management\n      rotation: >-\n        \"Create and rotate API keys in the hosted console.\" Rotation is self-serve; no rotation policy,\n        key lifetime, or expiry is published.\n      scopes: []\n      key_prefix: null\n      key_prefix_note: >-\n        No test/live key prefix convention is documented, and no sandbox/test key mode exists — a\n        WeaveAPI key is a live key. Not published, not inferable without an account.\n  verified_behavior:\n    method: probed\n    fetched: '2026-08-11'\n    observations:\n      - request: GET https://api.weaveapi.dev/v1/models with no Authorization header\n        status: 401\n        body: '{\"error\":{\"code\":\"\",\"message\":\"Invalid token (request id: …)\",\"type\":\"new_api_error\"}}'\n      - request: GET https://api.weaveapi.dev/v1/models with an invalid bearer token\n        status: 401\n        body: '{\"error\":{\"code\":\"\",\"message\":\"Invalid token (request\
  \ id: …)\",\"type\":\"new_api_error\"}}'\n        note: >-\n          A missing credential and a wrong credential are indistinguishable — both return the identical\n          401 \"Invalid token\". No WWW-Authenticate challenge header is returned on either.\n      - request: POST https://api.weaveapi.dev/v1/chat/completions with no Authorization header\n        status: 401\n    www_authenticate_header: false\n\n  anthropic_compatible_route:\n    base_url: https://api.weaveapi.dev\n    path: /v1/messages\n    auth: >-\n      Documented as the same WeaveAPI key. The Claude Code guide instructs the developer to set the base\n      URL WITHOUT /v1 because the client appends the messages path itself, and to place the key in the\n      CC Switch provider API Key field.\n    probed_status: 401\n    source: https://weaveapi.dev/docs/claude-code-cc-switch/\n\n# Console/account identity — human login to the hosted console. NOT API authorization.\nconsole_authentication:\n  method: probed\n  source:\
  \ https://api.weaveapi.dev/api/status\n  host: https://console.weaveapi.dev\n  methods:\n    - type: password\n      enabled: true\n      registration_enabled: true\n      email_verification_required: true\n    - type: oauth2\n      provider: GitHub\n      enabled: true\n      note: GitHub OAuth login for the console.\n    - type: openIdConnect\n      provider: Google\n      enabled: true\n      authorization_endpoint: https://accounts.google.com/o/oauth2/v2/auth\n      note: Google OIDC login for the console.\n    - type: webauthn\n      name: passkey\n      enabled: true\n      relying_party_id: console.weaveapi.dev\n      display_name: WeaveAPI\n      user_verification: preferred\n      note: >-\n        Passkey / WebAuthn login is supported on the console. This is the strongest authentication\n        control WeaveAPI operates, and it is on the human surface only.\n  bot_protection:\n    provider: Cloudflare Turnstile\n    enabled: true\n  mfa_for_api_keys: false\n  mfa_note: >-\n\
  \    No MFA, IP allowlisting, or key-scoping is documented for API keys themselves. Account access can be\n    hardened with a passkey; the credential that actually calls the API cannot be.\n\ngaps:\n  - No scopes or per-key permissions — one key grants the account's full API surface.\n  - No key expiry, TTL, or documented rotation policy.\n  - No test/live key separation and no key prefix convention.\n  - No WWW-Authenticate challenge on 401.\n  - No /.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource (both 404).\n  - Missing credential and invalid credential return identical responses.\n\nx-evidence:\n  - url: https://weaveapi.dev/docs/\n    http_status: 200\n  - url: https://api.weaveapi.dev/v1/models\n    http_status: 401\n  - url: https://api.weaveapi.dev/api/status\n    http_status: 200\n  - url: https://api.weaveapi.dev/.well-known/oauth-authorization-server\n    http_status: 404\n  - url: https://weaveapi.dev/docs/claude-code-cc-switch/\n    http_status:\
  \ 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weaveapi/refs/heads/main/authentication/weaveapi-authentication.yml
summary_line: apiKey · 0 schemes
tags:
- Artificial Intelligence
- LLM
- AI Inference
- API Gateway
- Aggregator
- OpenAI-Compatible
- Developer Tools
- Model Routing
- LLM Gateway
- prepaid credits
- Agent Tools
- Model Marketplace
---
