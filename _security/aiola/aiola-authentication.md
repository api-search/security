---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aiola Authentication
name_suffix: Authentication
oauth_flows: []
overview: aiOla declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: aiOla
provider_slug: aiola
scheme_count: 2
schemes:
- format: Bearer <api key>
  header: Authorization
  id: api_key
  in: header
  note: The docs are explicit that the API key must stay server-side and must never ship in frontend code or version control.
  obtained_from: https://platform.aiola.ai/
  obtained_from_status: unreachable 2026-09-14 — platform.aiola.ai is a dangling CNAME with no A record on any public resolver, so the documented route to a key does not resolve.
  scheme: bearer
  type: http
  used_for: the token-exchange call only (POST https://auth.aiola.ai/voip-auth/apiKey2Token)
- format: Bearer <JWT access token>
  header: Authorization
  id: access_token
  in: header
  lifetime: ~30 minutes (stated in the documentation FAQ)
  refresh: No refresh-token grant. A new access token is minted by repeating the API-key exchange. The SDKs cache the token and re-mint it when `exp` is within a 5-minute buffer.
  scheme: bearer
  token_format: JWT (RFC 7519) — the SDK parses the payload and reads `exp`
  type: http
  used_for: every Speech-to-Text and Text-to-Speech request, and the streaming Socket.IO handshake
slug: aiola-authentication
source_filename: aiola-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: https://docs.aiola.ai/developer-guides/authentication\ndocs: https://docs.aiola.ai/developer-guides/authentication\ncorroborated_by: https://github.com/aiola-lab/aiola-python-sdk (aiola/clients/auth/client.py,\n  aiola/constants.py)\nsummary: >-\n  Two-tier authentication. A long-lived API key never leaves the backend; it is exchanged\n  for a short-lived bearer token, which is exchanged for a session JWT access token bound\n  to a workflow. The access token is the credential every Speech API call carries.\nschemes:\n- id: api_key\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: Bearer <api key>\n  used_for: the token-exchange call only (POST https://auth.aiola.ai/voip-auth/apiKey2Token)\n  obtained_from: https://platform.aiola.ai/\n  obtained_from_status: >-\n    unreachable 2026-09-14 — platform.aiola.ai is a dangling CNAME with no A record on\n    any public resolver, so the documented route\
  \ to a key does not resolve.\n  note: The docs are explicit that the API key must stay server-side and must never ship\n    in frontend code or version control.\n- id: access_token\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: Bearer <JWT access token>\n  used_for: every Speech-to-Text and Text-to-Speech request, and the streaming Socket.IO\n    handshake\n  token_format: JWT (RFC 7519) — the SDK parses the payload and reads `exp`\n  lifetime: ~30 minutes (stated in the documentation FAQ)\n  refresh: >-\n    No refresh-token grant. A new access token is minted by repeating the API-key\n    exchange. The SDKs cache the token and re-mint it when `exp` is within a 5-minute\n    buffer.\nflow:\n- step: 1\n  operation: POST https://auth.aiola.ai/voip-auth/apiKey2Token\n  request_auth: Authorization Bearer <api key>\n  response_field: context.token\n  description: Exchanges the API key for a temporary bearer token.\n- step: 2\n  operation: POST https://auth.aiola.ai/voip-auth/session\n\
  \  request_auth: Authorization Bearer <temporary token>\n  request_body: '{ \"workflow_id\": \"<uuid>\" }'\n  response_fields:\n  - jwt\n  - sessionId\n  description: >-\n    Creates a session and returns the JWT access token plus a session id. A session\n    occupies a concurrency slot on the account.\n- step: 3\n  operation: DELETE https://auth.aiola.ai/voip-auth/session\n  request_auth: Authorization Bearer <access token>\n  response_fields:\n  - status\n  - deletedAt\n  description: >-\n    Closes the session and frees the concurrency slot. This is the explicit teardown an\n    agent must call; sessions are a metered resource, not a free handle.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes:\n  model: none\n  note: >-\n    No OAuth2 authorization server and no scope surface. A session is bound to a\n    workflow_id, which is a routing/configuration handle, not a permission scope, so no\n    scopes/ artifact is written.\nerrors:\n- status: 401\n  code: UNAUTHORIZED\n\
  \  message: Invalid or expired access token\n  remediation: Verify the Authorization header, confirm the `Bearer <token>` format, and\n    mint a new access token.\n- status: 403\n  code: FORBIDDEN\n  message: API key does not have required permissions\n  remediation: Confirm the API key is active and not revoked; contact aiOla support for\n    permission adjustments.\nkey_rotation: >-\n  Rotating the API key in the aiOla dashboard immediately invalidates every access token\n  minted from it.\nenvironments:\n  default_api_base: https://apis.aiola.ai\n  default_auth_base: https://auth.aiola.ai\n  enterprise: >-\n    Self-hosted / dedicated deployments override both bases — the docs show\n    https://your-company.api.aiola.ai + https://your-company.auth.aiola.ai and a\n    single-host https://your-company.aiola-enterprise.com form, configured through the\n    SDK's base_url / auth_base_url options or the AIOLA_ENDPOINT environment variable.\n  note: >-\n    The documentation's environment-variable\
  \ example still shows\n    AIOLA_ENDPOINT=https://api.aiola.com, a host that does not resolve; the SDK constant\n    shipped in the published packages is https://apis.aiola.ai. The docs and the code\n    disagree, and the code is the one that runs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiola/refs/heads/main/authentication/aiola-authentication.yml
summary_line: 2 schemes
tags:
- Speech Recognition
- Speech-to-Text
- Text-to-Speech
- Voice AI
- Conversational AI
- Artificial Intelligence
- Machine Learning
- Audio
- Transcription
- Enterprise
---
