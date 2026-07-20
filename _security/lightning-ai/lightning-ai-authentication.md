---
api_key_in:
- header
- environment
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Lightning Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lightning AI secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lightning AI
provider_slug: lightning-ai
scheme_count: 3
schemes:
- caveats:
  - Python SDK reads credentials at import time - setting os.environ after import is ignored. The JS SDK reads credentials lazily on each request.
  - A personal login key cannot be used where a teamspace-scoped key is required; sandbox creation fails with an explicit "not your personal login key" error.
  description: A Lightning API key authenticates the SDKs and the CLI against the platform control plane. Keys are created in the UI and can be scoped to a specific teamspace and role. The teamspace-scoped key is the recommended form - the key itself selects the project, so the JS SDK takes no teamspace argument.
  environment_variables:
  - name: LIGHTNING_SANDBOX_API_KEY
    role: Primary auth for Sandbox (preferred)
  - name: LIGHTNING_API_KEY
    role: Legacy / general platform fallback
  - name: LIGHTNING_USER_ID
    role: Paired with LIGHTNING_API_KEY for CLI environment auth
  - name: LIGHTNING_CLOUD_URL
    role: Optional control-plane base URL override (default https://lightning.ai)
  in_code:
  - example: Sandbox.configure(api_key="sk-lit-...", base_url="https://lightning.ai")
    language: python
  - example: 'Sandbox.configure({ apiKey: "sk-lit-...", baseUrl: "https://lightning.ai" })'
    language: javascript
  key_prefix: sk-lit-
  name: LightningApiKey
  precedence: Explicit configure() values -> LIGHTNING_SANDBOX_API_KEY -> LIGHTNING_API_KEY (legacy). For the base URL, configure({ baseUrl }) -> LIGHTNING_CLOUD_URL -> production default.
  provisioning: Organization settings -> Members -> API keys -> Create API Key
  scoping: teamspace + role
  type: apiKey
- command: lightning login
  description: The CLI can authenticate interactively via a browser-based login, which stores credentials locally for subsequent commands.
  name: InteractiveLogin
  type: interactive
- compatible_clients:
  - client: OpenAI Python SDK
  - client: Anthropic / Claude Code
    config: ANTHROPIC_BASE_URL=https://lightning.ai/ with ANTHROPIC_API_KEY set to the Lightning API key
  description: Lightning Model APIs authenticate with the same Lightning API key, passed to the litai client or supplied to OpenAI- and Anthropic-compatible clients as the API key with https://lightning.ai as the base URL.
  in_code:
  - example: LLM(model="openai/gpt-5", api_key="<LIGHTNING_API_KEY>")
    language: python
  name: ModelApiKey
  obtain_at: https://lightning.ai/lightning-ai/model-apis/models?showApiKey=true
  type: apiKey
slug: lightning-ai-authentication
source_filename: lightning-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://lightning.ai/docs/platform/developers/cli\ndocs:\n- https://lightning.ai/docs/platform/build/sandbox\n- https://lightning.ai/docs/platform/developers/sdk/sandbox/python-sandbox-sdk\n- https://lightning.ai/docs/platform/developers/sdk/sandbox/js-sandbox-sdk\n- https://lightning.ai/docs/platform/developers/cli\nnote: >-\n  Lightning AI publishes no OpenAPI definition, so this profile is captured from\n  the published SDK and CLI authentication documentation rather than derived from\n  securitySchemes. No OAuth 2.0 or OpenID Connect surface is documented for the\n  platform API, so there is no scopes/ artifact for this provider.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - environment\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: LightningApiKey\n  type: apiKey\n  description: >-\n    A Lightning API key authenticates the SDKs and the CLI against the platform\n\
  \    control plane. Keys are created in the UI and can be scoped to a specific\n    teamspace and role. The teamspace-scoped key is the recommended form - the\n    key itself selects the project, so the JS SDK takes no teamspace argument.\n  key_prefix: sk-lit-\n  scoping: teamspace + role\n  provisioning: Organization settings -> Members -> API keys -> Create API Key\n  environment_variables:\n  - name: LIGHTNING_SANDBOX_API_KEY\n    role: Primary auth for Sandbox (preferred)\n  - name: LIGHTNING_API_KEY\n    role: Legacy / general platform fallback\n  - name: LIGHTNING_USER_ID\n    role: Paired with LIGHTNING_API_KEY for CLI environment auth\n  - name: LIGHTNING_CLOUD_URL\n    role: Optional control-plane base URL override (default https://lightning.ai)\n  precedence: >-\n    Explicit configure() values -> LIGHTNING_SANDBOX_API_KEY ->\n    LIGHTNING_API_KEY (legacy). For the base URL, configure({ baseUrl }) ->\n    LIGHTNING_CLOUD_URL -> production default.\n  in_code:\n  - language:\
  \ python\n    example: 'Sandbox.configure(api_key=\"sk-lit-...\", base_url=\"https://lightning.ai\")'\n  - language: javascript\n    example: 'Sandbox.configure({ apiKey: \"sk-lit-...\", baseUrl: \"https://lightning.ai\" })'\n  caveats:\n  - >-\n    Python SDK reads credentials at import time - setting os.environ after\n    import is ignored. The JS SDK reads credentials lazily on each request.\n  - >-\n    A personal login key cannot be used where a teamspace-scoped key is\n    required; sandbox creation fails with an explicit \"not your personal login\n    key\" error.\n- name: InteractiveLogin\n  type: interactive\n  description: >-\n    The CLI can authenticate interactively via a browser-based login, which\n    stores credentials locally for subsequent commands.\n  command: lightning login\n- name: ModelApiKey\n  type: apiKey\n  description: >-\n    Lightning Model APIs authenticate with the same Lightning API key, passed to\n    the litai client or supplied to OpenAI- and Anthropic-compatible\
  \ clients as\n    the API key with https://lightning.ai as the base URL.\n  obtain_at: https://lightning.ai/lightning-ai/model-apis/models?showApiKey=true\n  in_code:\n  - language: python\n    example: LLM(model=\"openai/gpt-5\", api_key=\"<LIGHTNING_API_KEY>\")\n  compatible_clients:\n  - client: OpenAI Python SDK\n  - client: Anthropic / Claude Code\n    config: ANTHROPIC_BASE_URL=https://lightning.ai/ with ANTHROPIC_API_KEY set\n      to the Lightning API key\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightning-ai/refs/heads/main/authentication/lightning-ai-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Ai Ml
- Machine Learning
- GPU Cloud
- Model Inference
- Model Training
- Developer Platform
- Sandboxes
- LLM APIs
- Open Source
---
