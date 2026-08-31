---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Formality Authentication
name_suffix: Authentication
oauth_flows: []
overview: Formality secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Formality
provider_slug: formality
scheme_count: 2
schemes:
- format: 'Authorization: Bearer <your-refresh-token>'
  header: Authorization
  in: header
  issued_by: Personal Settings > Formality API > New Token
  lifetime: operator-chosen, "from a few days to a full year"
  name: refreshToken
  note: A long-lived PERSONAL refresh token. It is not used to call resource endpoints; its only documented purpose is to be exchanged at GET /api/v1/token for a short-lived access token. Because it is minted per user in Personal Settings, an integration inherits that individual's permissions — Formality documents no separate service-account or machine credential.
  revocable: true
  role: credential
  scheme: bearer
  shown_once: true
  sources:
  - https://help.formality.com/integrations/api
  type: http
  usage_visibility: The token list shows when and where each token was last used.
- format: 'Authorization: Bearer <your-access-token>'
  header: Authorization
  in: header
  lifetime_note: '"The access token has a lifespan of 5 minutes, once expired you''ll need to generate a new one." No refresh-token rotation, expiry hint or Retry-After style signal is documented, so a client must either re-exchange before every call or handle a 401 and retry.'
  lifetime_seconds: 300
  name: accessToken
  obtained_from: GET /api/v1/token
  response_shape: '{"token": "<access token>"}'
  role: access
  scheme: bearer
  sources:
  - https://help.formality.com/integrations/api
  type: http
slug: formality-authentication
source_filename: formality-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: https://help.formality.com/integrations/api\ndocs: https://help.formality.com/integrations/api\nnote: >-\n  Derived by hand from the help centre, not from an OpenAPI document. Formality\n  publishes a Swagger UI at https://app.eu1.formality.com/-/api-doc-swagger but it\n  HTTP 302s to https://auth.eu1.formality.com/?callbackUrl=..., and\n  /api/v1/openapi.json and /api/v1/swagger.json both return 401, so no\n  securitySchemes block could be read. Everything below is stated verbatim in\n  Formality's own API documentation.\nsummary:\n  types: [http]\n  api_key_in: []\n  oauth2_flows: []\n  scheme: bearer\n  token_exchange: true\n  end_user_sso: [Google, Microsoft]\nschemes:\n- name: refreshToken\n  type: http\n  scheme: bearer\n  role: credential\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer <your-refresh-token>'\n  issued_by: Personal Settings > Formality API > New Token\n  lifetime: operator-chosen,\
  \ \"from a few days to a full year\"\n  revocable: true\n  shown_once: true\n  usage_visibility: >-\n    The token list shows when and where each token was last used.\n  sources: [https://help.formality.com/integrations/api]\n  note: >-\n    A long-lived PERSONAL refresh token. It is not used to call resource endpoints;\n    its only documented purpose is to be exchanged at GET /api/v1/token for a\n    short-lived access token. Because it is minted per user in Personal Settings, an\n    integration inherits that individual's permissions — Formality documents no\n    separate service-account or machine credential.\n- name: accessToken\n  type: http\n  scheme: bearer\n  role: access\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer <your-access-token>'\n  obtained_from: GET /api/v1/token\n  lifetime_seconds: 300\n  lifetime_note: >-\n    \"The access token has a lifespan of 5 minutes, once expired you'll need to\n    generate a new one.\" No refresh-token rotation,\
  \ expiry hint or Retry-After style\n    signal is documented, so a client must either re-exchange before every call or\n    handle a 401 and retry.\n  response_shape: '{\"token\": \"<access token>\"}'\n  sources: [https://help.formality.com/integrations/api]\nflow:\n  style: two-step bearer exchange\n  steps:\n  - step: 1\n    action: Create a personal Refresh Token in Personal Settings > Formality API\n    note: The full token is displayed only once at creation.\n  - step: 2\n    action: 'GET /api/v1/token with header: Authorization: Bearer <refresh-token>'\n    returns: 'JSON body {\"token\": \"...\"} containing the 5-minute access token'\n  - step: 3\n    action: 'Call resource endpoints with Authorization: Bearer <access-token>'\nscoping:\n  model: workspace-path\n  note: >-\n    Authorization is scoped by the workspaceId path segment rather than by token\n    scopes. The workspaceId is the slug that follows the application host in the app\n    URL (app URL .../myCompany/agreements\
  \ => workspaceId \"myCompany\"), and it is a\n    required segment of every resource path. There is no OAuth authorization server,\n    no scope vocabulary and no consent screen, which is why scopes/ was deliberately\n    not written for this provider.\nend_user_authentication:\n  sso: [Microsoft, Google]\n  magic_link: true\n  enforce_sso_toggle: true\n  enforce_sso_note: >-\n    An \"Imposer la connexion SSO\" toggle in workspace Security settings blocks\n    magic-link sign-in and terminates existing non-SSO sessions, forcing\n    re-authentication through Google or Microsoft.\n  allowed_email_domains: true\n  source: https://help.formality.com/setup-permissions/user-management\n  note: >-\n    This is human sign-in to the application, NOT API authentication. It is recorded\n    because the Swagger UI is gated behind it.\nobserved_behaviour:\n- url: https://app.eu1.formality.com/api/v1/token\n  status: 401\n  fetched: '2026-08-17'\n- url: https://app.eu1.formality.com/api/v1/demo/agreements\n\
  \  status: 401\n  fetched: '2026-08-17'\n- url: https://app.eu1.formality.com/api/v1/openapi.json\n  status: 401\n  fetched: '2026-08-17'\n- url: https://app.eu1.formality.com/-/api-doc-swagger\n  status: 302\n  location: https://auth.eu1.formality.com?callbackUrl=https://app.eu1.formality.com/-/api-doc-swagger\n  fetched: '2026-08-17'\ncaveat: >-\n  The 401 responses above are a BLANKET gate, not endpoint confirmation: a\n  deliberately nonsensical path\n  (/api/v1/nonexistentgarbagexyz/zzznotreal) also returns 401 with the same 17-byte\n  \"401 Unauthorized\" body. Unauthenticated probing therefore proves the /api/v1/\n  surface is live and auth-gated, but it cannot confirm which individual endpoints\n  exist. Every endpoint recorded in this repo comes from Formality's published\n  documentation, not from probe inference.\ngaps:\n- No OpenAPI/Swagger document is reachable without a session.\n- No /.well-known/openid-configuration or oauth-authorization-server is served.\n- No documented\
  \ token-rotation, key-prefix or sandbox-vs-live credential separation.\n- No documented rate limit or 429 behaviour on the token-exchange endpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formality/refs/heads/main/authentication/formality-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Ai/Ml
- Legal
- Contract Management
- Document-Management
- Asset Intelligence
- Compliance
- Software-as-a-Service
---
