---
anonymous_access: false
api_key_in: []
api_specs:
- filename: umami-authentication-api-openapi.yml
  format: yaml
  label: Umami Authentication API
  slug: umami-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-authentication-api-openapi.yml
- filename: umami-teams-api-openapi.yml
  format: yaml
  label: Umami Teams API
  slug: umami-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-teams-api-openapi.yml
- filename: umami-users-api-openapi.yml
  format: yaml
  label: Umami Users API
  slug: umami-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-users-api-openapi.yml
- filename: umami-websites-api-openapi.yml
  format: yaml
  label: Umami Websites API
  slug: umami-websites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-websites-api-openapi.yml
- filename: umami-account-api-openapi.yml
  format: yaml
  label: Umami Account API
  slug: umami-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-account-api-openapi.yml
- filename: umami-administration-api-openapi.yml
  format: yaml
  label: Umami Administration API
  slug: umami-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-administration-api-openapi.yml
- filename: umami-boards-api-openapi.yml
  format: yaml
  label: Umami Boards API
  slug: umami-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-boards-api-openapi.yml
- filename: umami-collection-api-openapi.yml
  format: yaml
  label: Umami Collection API
  slug: umami-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-collection-api-openapi.yml
- filename: umami-dashboard-api-openapi.yml
  format: yaml
  label: Umami Dashboard API
  slug: umami-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-dashboard-api-openapi.yml
- filename: umami-links-api-openapi.yml
  format: yaml
  label: Umami Links API
  slug: umami-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-links-api-openapi.yml
- filename: umami-pixels-api-openapi.yml
  format: yaml
  label: Umami Pixels API
  slug: umami-pixels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-pixels-api-openapi.yml
- filename: umami-realtime-api-openapi.yml
  format: yaml
  label: Umami Realtime API
  slug: umami-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-realtime-api-openapi.yml
- filename: umami-scripts-api-openapi.yml
  format: yaml
  label: Umami Scripts API
  slug: umami-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-scripts-api-openapi.yml
- filename: umami-shares-api-openapi.yml
  format: yaml
  label: Umami Shares API
  slug: umami-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-shares-api-openapi.yml
- filename: umami-system-api-openapi.yml
  format: yaml
  label: Umami System API
  slug: umami-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-system-api-openapi.yml
- filename: umami-two-factor-authentication-api-openapi.yml
  format: yaml
  label: Umami Two-factor authentication API
  slug: umami-two-factor-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-two-factor-authentication-api-openapi.yml
auth_types:
- http
description: Umami has two distinct authentication paths that share one wire format. Both send a bearer credential in the Authorization header, but they are obtained differently, live on different hosts, and are not interchangeable.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Umami Authentication
name_suffix: Authentication
oauth_flows: []
overview: Umami secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Umami
provider_slug: umami
scheme_count: 2
schemes:
- description: 'An API key generated in the Umami Cloud UI (Settings → API keys → Create key) and sent as `Authorization: Bearer <api-key>`. This is the only way to reach Umami Cloud programmatically.'
  docs: https://docs.umami.is/docs/cloud/api-key
  host: https://api.umami.is/v1
  name: cloudApiKey
  obtained_by: manual creation in the Umami Cloud dashboard
  plan_gated: true
  plan_note: API access is NOT available on the free Hobby plan. It starts at Pro ($20/month). This is an access-model fact, not just a pricing one.
  programmatic_issuance: false
  rate_limit: 50 calls per 15 seconds per key (see rate-limits/)
  regions:
    default: the region of the account that owns the key
    form: https://api.umami.is/v1/us | https://api.umami.is/v1/eu
    pinnable: true
  restrictions:
  - 'The following routes are NOT available to an API key, even a valid one: /me/password, /users, /users/*. User administration is UI-only on Cloud.'
  rotation: Keys can be deleted from the API keys screen; deletion is irreversible. No documented expiry, no documented rotation API.
  scheme: bearer
  source: https://docs.umami.is/docs/cloud/api-key
  surface: Umami Cloud
  type: http
- bearerFormat: JWT
  description: 'A JWT obtained by POSTing username/password to /api/auth/login, then sent as `Authorization: Bearer <token>` on every subsequent call. Applies to self-hosted instances only — Umami Cloud does not use it.'
  docs: https://docs.umami.is/docs/api/authentication
  expiry: not documented
  host: http://<your-umami-instance>/api
  logout: POST /api/auth/logout
  name: selfHostedJwt
  obtained_by: POST /api/auth/login
  rotation: re-login
  scheme: bearer
  source: https://docs.umami.is/docs/api/authentication
  surface: self-hosted Umami
  type: http
  verify: POST /api/auth/verify returns the token's user, or fails if expired.
slug: umami-authentication
source_filename: umami-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.umami.is/docs/api/authentication + https://docs.umami.is/docs/cloud/api-key\ndocs: https://docs.umami.is/docs/api/authentication\nprovider: Umami\nproviderId: umami\ndescription: Umami has two distinct authentication paths that share one wire format. Both send a bearer credential in the Authorization header, but they are obtained differently, live on different hosts,\n  and are not interchangeable.\nsummary:\n  types:\n  - http\n  schemes_count: 2\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  note: 'No OAuth 2.0, no OpenID Connect, no scopes, no mTLS. There is nothing to delegate: a Umami credential is all-or-nothing for the account or user it belongs to. See scopes/ — no OAuthScopes artifact\n    is emitted because there are no scopes to record.'\nschemes:\n- name: cloudApiKey\n  type: http\n  scheme: bearer\n  surface: Umami Cloud\n  host: https://api.umami.is/v1\n  description: 'An API key generated\
  \ in the Umami Cloud UI (Settings → API keys → Create key) and sent as `Authorization: Bearer <api-key>`. This is the only way to reach Umami Cloud programmatically.'\n  obtained_by: manual creation in the Umami Cloud dashboard\n  programmatic_issuance: false\n  rotation: Keys can be deleted from the API keys screen; deletion is irreversible. No documented expiry, no documented rotation API.\n  plan_gated: true\n  plan_note: API access is NOT available on the free Hobby plan. It starts at Pro ($20/month). This is an access-model fact, not just a pricing one.\n  restrictions:\n  - 'The following routes are NOT available to an API key, even a valid one: /me/password, /users, /users/*. User administration is UI-only on Cloud.'\n  regions:\n    default: the region of the account that owns the key\n    pinnable: true\n    form: https://api.umami.is/v1/us | https://api.umami.is/v1/eu\n  rate_limit: 50 calls per 15 seconds per key (see rate-limits/)\n  docs: https://docs.umami.is/docs/cloud/api-key\n\
  \  source: https://docs.umami.is/docs/cloud/api-key\n- name: selfHostedJwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  surface: self-hosted Umami\n  host: http://<your-umami-instance>/api\n  description: 'A JWT obtained by POSTing username/password to /api/auth/login, then sent as `Authorization: Bearer <token>` on every subsequent call. Applies to self-hosted instances only — Umami Cloud\n    does not use it.'\n  obtained_by: POST /api/auth/login\n  verify: POST /api/auth/verify returns the token's user, or fails if expired.\n  logout: POST /api/auth/logout\n  expiry: not documented\n  rotation: re-login\n  docs: https://docs.umami.is/docs/api/authentication\n  source: https://docs.umami.is/docs/api/authentication\nunauthenticated_endpoints:\n- path: POST /api/send\n  reason: Data collection. Requires no token but DOES require a valid User-Agent header or the request is not registered. Umami Cloud collection posts to gateway.umami.is as of 2026-06-06 (previously cloud.umami.is/api/send).\n\
  \  source: https://docs.umami.is/docs/api/sending-stats\n- path: POST /api/batch\n  reason: Batched collection; same rules as /api/send.\n  source: https://docs.umami.is/docs/api/sending-stats\n- path: GET /api/websites/:websiteId/recorder\n  reason: 'Recorder configuration read by the tracker to initialize session replay and heatmaps. Documented as publicly accessible with no authentication. Returns {\"enabled\": false} when the website does\n    not exist or recording is off.'\n  source: https://docs.umami.is/docs/api/websites\n- path: /share/:shareId\n  reason: Share URLs render a dashboard to anyone holding the link. shareId is set per website and can be revoked by setting it to null.\n  source: https://docs.umami.is/docs/enable-share-url\naccount_security:\n  two_factor:\n    supported: true\n    surface: application login (self-hosted and Cloud)\n    enforcement: Can be enforced globally by an admin and per team; API routes exist at /api/2fa/* and /api/admin/2fa/global.\n    docs:\
  \ https://docs.umami.is/docs/two-factor-authentication\n    note: TOTP protects interactive login. It does not gate API-key use.\n  sso:\n    supported: true\n    protocol: SAML\n    availability: Enterprise plan only\n    source: https://umami.is/pricing\nobserved:\n- probe: GET https://api.umami.is/v1/websites (no credential)\n  status: 400\n  body: '{\"error\":{\"message\":\"No API key specified.\",\"code\":\"bad-request\",\"status\":400}}'\n  date: '2026-08-13'\n- probe: GET https://api.umami.is/v1/websites (Authorization Bearer <invalid>)\n  status: 401\n  body: '{\"error\":{\"message\":\"Invalid API key.\",\"code\":\"unauthorized\",\"status\":401}}'\n  date: '2026-08-13'\n  note: Missing credential is answered 400, not 401 — worth knowing for client error handling, since most APIs return 401 for both.\nprior_state: Superseded the 2026-07-11 derived profile, which recorded a single bearerAuth scheme from the scaffold OpenAPI and conflated the Cloud API key with the self-hosted JWT\
  \ into one description.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\ndocs_pages:\n- https://docs.umami.is/docs/api/authentication\n- https://docs.umami.is/docs/cloud/api-key\n- https://docs.umami.is/docs/two-factor-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/authentication/umami-authentication.yml
summary_line: http · 2 schemes
tags:
- Cookieless Tracking
- Open Source
- Privacy
- Web Analytics
- Website Analytics
- Product Analytics
- Event Tracking
- Self-Hosted
- GDPR
- Session Replay
- Heatmaps
- Marketing Attribution
---
