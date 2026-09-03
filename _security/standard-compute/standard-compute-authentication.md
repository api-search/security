---
api_key_in: []
api_specs:
- filename: standard-compute-openapi.json
  format: json
  label: Standard Compute Inference API
  slug: standard-compute-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-compute/refs/heads/main/openapi/standard-compute-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Standard Compute Authentication
name_suffix: Authentication
oauth_flows: []
overview: Standard Compute declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Standard Compute
provider_slug: standard-compute
scheme_count: 1
schemes:
- applies_to:
  - POST /v1/chat/completions
  - POST /v1/completions
  - POST /v1/responses
  - POST /v1/messages
  - POST /v1/messages/count_tokens
  format: 'Authorization: Bearer <key>'
  header: Authorization
  id: bearerApiKey
  in: header
  issued_from: dashboard (https://standardcompute.com/dashboard)
  key_prefix: sc_live_
  key_prefix_source: https://standardcompute.com/getting-started
  rotation: Plaintext key is displayed exactly once at creation; only an encrypted blob and the last four characters are retained afterwards, and the provider states there is no administrative path to recover the plaintext. Rotation therefore means issuing a new key.
  scheme: bearer
  storage_guidance: Docs instruct storing the key in the platform secrets store rather than hardcoding it.
  type: http
slug: standard-compute-authentication
source_filename: standard-compute-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://standardcompute.com/getting-started\ndocs: https://standardcompute.com/getting-started\nalso:\n  - https://standardcompute.com/security\n  - https://standardcompute.com/support\n  - probed: POST https://api.stdcmpt.com/v1/chat/completions (no key) -> HTTP 401\nsummary: >-\n  Single-credential Bearer API key. There is no OAuth, no OIDC, no mTLS and no\n  scope model — one long-lived account key authenticates every operation on\n  https://api.stdcmpt.com/v1. Because the surface is OpenAI-wire-compatible, the\n  key is supplied exactly the way an OpenAI key is, which is the whole point:\n  agents swap the base URL and the key and nothing else changes.\nschemes:\n  - id: bearerApiKey\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: \"Authorization: Bearer <key>\"\n    key_prefix: sc_live_\n    key_prefix_source: https://standardcompute.com/getting-started\n    issued_from: dashboard\
  \ (https://standardcompute.com/dashboard)\n    rotation: >-\n      Plaintext key is displayed exactly once at creation; only an encrypted blob\n      and the last four characters are retained afterwards, and the provider states\n      there is no administrative path to recover the plaintext. Rotation therefore\n      means issuing a new key.\n    storage_guidance: >-\n      Docs instruct storing the key in the platform secrets store rather than\n      hardcoding it.\n    applies_to:\n      - POST /v1/chat/completions\n      - POST /v1/completions\n      - POST /v1/responses\n      - POST /v1/messages\n      - POST /v1/messages/count_tokens\nanonymous_operations:\n  - path: /v1/models\n    method: GET\n    note: >-\n      Confirmed unauthenticated on 2026-09-02 (HTTP 200, model list returned). The\n      provider's own status page documents this as the self-service uptime check.\n  - path: /install.sh\n    method: GET\n    note: Setup script, served without authentication (HTTP 200).\n\
  \  - path: /install.ps1\n    method: GET\nalternate_env_conventions:\n  - description: >-\n      OpenAI-compatible agents read the standard OpenAI variables.\n    variables:\n      OPENAI_BASE_URL: https://api.stdcmpt.com/v1\n      OPENAI_API_KEY: \"<Standard Compute key>\"\n      OPENAI_MODEL: standardcompute\n  - description: >-\n      Anthropic-compatible agents (Claude Code) read the Anthropic variables, and\n      the base URL deliberately drops the /v1 suffix because the client appends\n      /v1/messages itself.\n    variables:\n      ANTHROPIC_BASE_URL: https://api.stdcmpt.com\n      ANTHROPIC_API_KEY: \"<Standard Compute key>\"\n    source: https://standardcompute.com/integrations/claude-code\nkey_verification:\n  method: HMAC-SHA256 over the submitted key compared against the stored hash\n  constant_time_compare: true\n  at_rest_encryption: AES-256-GCM, per-account derived key stored separately\n  brute_force_control: failed authentication attempts are rate limited\n  source:\
  \ https://standardcompute.com/security\ntransport:\n  tls_minimum: '1.2'\n  plaintext_http: refused (not redirected or downgraded)\n  profile: Mozilla Intermediate\n  source: https://standardcompute.com/security\nfailure_modes:\n  - status: 401\n    body: '{\"error\": {\"message\": \"Invalid API key\", \"type\": \"invalid_request_error\"}}'\n    observed: '2026-09-02'\n    note: Observed live against POST /v1/chat/completions with no Authorization header.\ngaps:\n  - >-\n    The published OpenAPI (https://api.stdcmpt.com/openapi.json) declares NO\n    components.securitySchemes and no security requirement on any operation, even\n    though every /v1 completion path requires a Bearer key. An agent reading only\n    the spec would believe the API is anonymous. This is captured as a correction\n    in overlays/standard-compute-openapi-overlay.yaml and is the single highest-value\n    fix the provider could make to their contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/standard-compute/refs/heads/main/authentication/standard-compute-authentication.yml
summary_line: 1 scheme
tags:
- llm api
- flat-rate
- subscription
- ai agents
- inference
- model routing
- ai gateway
- developer tools
- coding agents
- openai-compatible
---
