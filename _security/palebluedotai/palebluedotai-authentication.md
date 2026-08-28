---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Palebluedotai Authentication
name_suffix: Authentication
oauth_flows: []
overview: PaleBlueDot.AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: PaleBlueDot.AI
provider_slug: palebluedotai
scheme_count: 2
schemes:
- applies_to: Inference API (/v1/chat/completions, /v1/responses, /v1/messages, /v1beta/..., /v1/images/generations, /v1/video/generations)
  format: Bearer <API_KEY>
  header: Authorization
  id: inference_api_key
  in: header
  issued_via: TokenRouter Console -> API Keys -> Create Key
  key_format: sk-xxxxxxxxxxxxxxxx
  key_prefix: sk-
  notes:
  - Anthropic-compatible clients pass the same key as ANTHROPIC_AUTH_TOKEN with ANTHROPIC_BASE_URL=https://api.tokenrouter.com (no /v1 suffix).
  - OpenAI-compatible clients use base URL https://api.tokenrouter.com/v1.
  - Per-key spend quota and enable/disable state are managed through the Management API.
  scheme: bearer
  scoped: false
  source: https://www.tokenrouter.com/docs/openclaw-setup/
  type: http
- applies_to: Management API (/api/management/*)
  distinct_from_inference_key: true
  format: Bearer <YOUR_MANAGEMENT_KEY>
  header: Authorization
  id: management_key
  in: header
  middleware: ManagementKeyForAuth
  notes:
  - A Management Key is a separate credential from an inference API key; it resolves to its owning user and, for enterprise super administrators, to the whole organization.
  - Keys carry a status (enabled/disabled) and an ExpiresTime.
  scheme: bearer
  source: https://www.tokenrouter.com/docs/management-api-documentation/
  type: http
slug: palebluedotai-authentication
source_filename: palebluedotai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://www.tokenrouter.com/docs/management-api-documentation/\nname: PaleBlueDot.AI / PBD TokenRouter authentication\nnote: >-\n  Derived from the provider's published Management API reference and the agent-setup\n  guides, then confirmed against live unauthenticated responses. There is no published\n  OpenAPI document, so these schemes are transcribed from prose docs and from observed\n  401 bodies rather than from a machine-readable securitySchemes block.\nownership_note: >-\n  TokenRouter is on a different domain from palebluedot.ai. It is PaleBlueDot AI's own\n  product: PaleBlueDot AI announced PBD TokenRouter by press release, tokenrouter.com's\n  footer links to PaleBlueDot AI's LinkedIn/YouTube/X accounts, and the gateway's own\n  anonymous https://api.tokenrouter.com/api/status response embeds\n  \"https://www.palebluedot.ai/open/chat/\" and a palebluedot.ai logo URL. The TokenRouter\n  Terms of Use name Artemis Tokenrouter\
  \ Inc. as the operating entity.\nhosts:\n- https://api.tokenrouter.com\nschemes:\n- id: inference_api_key\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <API_KEY>'\n  key_prefix: sk-\n  key_format: sk-xxxxxxxxxxxxxxxx\n  applies_to: Inference API (/v1/chat/completions, /v1/responses, /v1/messages, /v1beta/..., /v1/images/generations, /v1/video/generations)\n  issued_via: TokenRouter Console -> API Keys -> Create Key\n  scoped: false\n  notes:\n  - Anthropic-compatible clients pass the same key as ANTHROPIC_AUTH_TOKEN with ANTHROPIC_BASE_URL=https://api.tokenrouter.com (no /v1 suffix).\n  - OpenAI-compatible clients use base URL https://api.tokenrouter.com/v1.\n  - Per-key spend quota and enable/disable state are managed through the Management API.\n  source: https://www.tokenrouter.com/docs/openclaw-setup/\n- id: management_key\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <YOUR_MANAGEMENT_KEY>'\n  applies_to:\
  \ Management API (/api/management/*)\n  middleware: ManagementKeyForAuth\n  distinct_from_inference_key: true\n  notes:\n  - A Management Key is a separate credential from an inference API key; it resolves to its owning user and, for enterprise super administrators, to the whole organization.\n  - Keys carry a status (enabled/disabled) and an ExpiresTime.\n  source: https://www.tokenrouter.com/docs/management-api-documentation/\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes_published: false\nscopes_note: >-\n  No OAuth2 or scope surface is published. The gateway's own /api/status response reports\n  oidc_enabled false, github_oauth false, discord_oauth false and wechat_login false,\n  so scopes/ is intentionally not emitted.\nfailure_modes:\n- http_status: 401\n  message: No Authorization request header provided\n  cause: Missing Authorization header.\n- http_status: 401\n  message: management key is invalid\n  cause: Key not found or soft-deleted.\n- http_status: 403\n\
  \  message: management key has been disabled\n  cause: Key status is not enabled.\n- http_status: 403\n  message: management key has expired\n  cause: Key past its ExpiresTime.\n- http_status: 403\n  message: User has been banned\n  cause: Owning user is not enabled.\nx-evidence:\n- url: https://api.tokenrouter.com/api/management/api-keys\n  method: GET\n  http_status: 401\n  body: '{\"message\":\"No Authorization request header provided\",\"success\":false}'\n  note: Live unauthenticated response matches the documented failure message verbatim.\n  fetched: '2026-08-26'\n- url: https://api.tokenrouter.com/v1/models\n  method: GET\n  http_status: 401\n  body: '{\"error\":{\"code\":\"\",\"message\":\"Token not provided (request id: ...)\",\"type\":\"api_error\"}}'\n  fetched: '2026-08-26'\n- url: https://api.palebluedot.ai/\n  method: GET\n  http_status: 401\n  body: '{\"error\": {\"message\": \"invalid or missing API key\", \"type\": \"authentication_error\"}}'\n  note: A second, separately-branded\
  \ gateway host also owned by the provider; every path returns this same 401, so no anonymous discovery is possible there.\n  fetched: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/palebluedotai/refs/heads/main/authentication/palebluedotai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Machine Learning
- Large Language Models
- Inference
- API Gateway
- GPU
- Cloud Computing
- Model Routing
- Compute
- Company
---
