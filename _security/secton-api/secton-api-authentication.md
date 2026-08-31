---
api_key_in:
- header
api_specs:
- filename: secton-api-chat-api-openapi.yml
  format: yaml
  label: Secton API Chat API
  slug: secton-api-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/secton-api/refs/heads/main/openapi/secton-api-chat-api-openapi.yml
- filename: secton-api-models-api-openapi.yml
  format: yaml
  label: Secton API Models API
  slug: secton-api-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/secton-api/refs/heads/main/openapi/secton-api-models-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Secton Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Secton API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Secton API
provider_slug: secton-api
scheme_count: 1
schemes:
- expiry: Keys can expire or be revoked — the live 401 reads "Invalid or expired API key" — but no lifetime or expiry policy is published.
  in: header
  issuance_requires_account: true
  issuance_url: https://console.secton.org/api
  key_prefix: not published, and not observable without an account
  name: ApiKeyAuth
  parameter: Authorization
  rotation: Console Terms §6 makes the customer responsible for "promptly rotating compromised credentials"; the rotation mechanism itself is inside the console and is not documented publicly.
  sdk_env_var: SECTON_API_KEY
  sdk_source: npm `secton` 1.0.2 README
  sources:
  - openapi/secton-api-chat-api-openapi.yml
  - openapi/secton-api-models-api-openapi.yml
  transmitted_as:
    also_accepted: 'Authorization: Bearer <api key>'
    documented: 'Authorization: <api key>'
    evidence: Both forms returned the same `{"error":"Invalid or expired API key"}` 401 when probed with a fabricated value on 2026-08-16, so the server tolerates either. The live "API key is missing from bearer" message implies bearer is the intended form, which contradicts the OpenAPI's raw-apiKey declaration.
  type: apiKey
slug: secton-api-authentication
source_filename: secton-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: searched\nsource: >-\n  openapi/secton-api-chat-api-openapi.yml, openapi/secton-api-models-api-openapi.yml (derived\n  baseline via derive-authentication.py); upgraded from https://secton.org/legal/console-terms §6,\n  the first-party npm `secton` 1.0.2 README, and live probes of\n  https://api.secton.org/v1/models and /v1/chat/completions (2026-08-16)\ndocs: https://console.secton.org/api\ndocs_note: >-\n  The key-issuance page is a JavaScript-rendered console behind login — nothing about\n  authentication is readable there without an account. There is no public auth documentation page.\n  Every field below is evidenced from the OpenAPI, the Console Terms, the SDK, or a live response.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2: false\n  oidc: false\n  mtls: false\n  scopes: false\n  scopes_note: >-\n    No scope or permission surface exists — the credential is all-or-nothing. scopes/ is\n    deliberately not written;\
  \ forcing an empty OAuth-scope artifact would misrepresent the model.\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: Authorization\n    sources:\n      - openapi/secton-api-chat-api-openapi.yml\n      - openapi/secton-api-models-api-openapi.yml\n    issuance_url: https://console.secton.org/api\n    issuance_requires_account: true\n    key_prefix: not published, and not observable without an account\n    rotation: >-\n      Console Terms §6 makes the customer responsible for \"promptly rotating compromised\n      credentials\"; the rotation mechanism itself is inside the console and is not documented\n      publicly.\n    expiry: >-\n      Keys can expire or be revoked — the live 401 reads \"Invalid or expired API key\" — but no\n      lifetime or expiry policy is published.\n    transmitted_as:\n      documented: 'Authorization: <api key>'\n      also_accepted: 'Authorization: Bearer <api key>'\n      evidence: >-\n        Both forms returned the same\
  \ `{\"error\":\"Invalid or expired API key\"}` 401 when probed with\n        a fabricated value on 2026-08-16, so the server tolerates either. The live \"API key is\n        missing from bearer\" message implies bearer is the intended form, which contradicts the\n        OpenAPI's raw-apiKey declaration.\n    sdk_env_var: SECTON_API_KEY\n    sdk_source: npm `secton` 1.0.2 README\nspec_defect:\n  issue: security is declared but never applied\n  detail: >-\n    The source document places the security requirement at `components.security`, which is not a\n    valid OpenAPI location — the requirement belongs at the document root or on each operation.\n    `components.securitySchemes.ApiKeyAuth` is defined correctly, but no operation references it.\n    A client generated from the published spec will therefore send NO credential and receive 401\n    on every call.\n  evidence: openapi/_original/secton-api-openapi.json\n  remediation: \"overlays/secton-api-chat-api-overlay.yaml and overlays/secton-api-models-api-overlay.yaml\
  \ add `security: [{ApiKeyAuth: []}]` at the root of each refined spec.\"\ncustomer_obligations:\n  source: https://secton.org/legal/console-terms §6 (effective 2026-08-06)\n  obligations:\n    - maintain the confidentiality of credentials\n    - implement appropriate security controls\n    - monitor usage associated with credentials\n    - promptly rotate compromised credentials\n    - limit access to authorized persons\n  prohibitions:\n    - credentials may not be shared publicly\n    - credentials may not be embedded in publicly accessible source code\n    - credentials may not be sold, leased, sublicensed or transferred\n  attribution: >-\n    \"Activity performed using credentials issued to a workspace or Account may be attributed to the\n    applicable Customer.\"\nbrowser_exposure_risk:\n  cors_allows_authorization: true\n  observed:\n    access-control-allow-origin: '*'\n    access-control-allow-headers: Content-Type, Authorization\n  note: >-\n    Wildcard CORS plus an allowed\
  \ `Authorization` header means the API is callable straight from a\n    browser with a raw key, and the SDK README demonstrates exactly that with an unpinned\n    `<script type=\"module\">` import from unpkg. Doing so publishes the key to every visitor and\n    breaches Secton's own Console Terms §6. Consumers should proxy server-side.\ndiscovery:\n  oauth_authorization_server: not-served (404 / soft-404 on every host)\n  oauth_protected_resource: not-served\n  openid_configuration: not-served\n  see: well-known/secton-api-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/secton-api/refs/heads/main/authentication/secton-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Inference
- llm
- chat-completions
- generative-ai
- Developer Tools
- openai-compatible
- streaming
- machine-learning
---
