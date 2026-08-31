---
api_key_in:
- header
api_specs:
- filename: listmonk-bounces-api-openapi.yml
  format: yaml
  label: listmonk Bounces API
  slug: listmonk-bounces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-bounces-api-openapi.yml
- filename: listmonk-campaigns-api-openapi.yml
  format: yaml
  label: listmonk Campaigns API
  slug: listmonk-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-campaigns-api-openapi.yml
- filename: listmonk-import-api-openapi.yml
  format: yaml
  label: listmonk Import API
  slug: listmonk-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-import-api-openapi.yml
- filename: listmonk-lists-api-openapi.yml
  format: yaml
  label: listmonk Lists API
  slug: listmonk-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-lists-api-openapi.yml
- filename: listmonk-media-api-openapi.yml
  format: yaml
  label: listmonk Media API
  slug: listmonk-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-media-api-openapi.yml
- filename: listmonk-subscribers-api-openapi.yml
  format: yaml
  label: listmonk Subscribers API
  slug: listmonk-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-subscribers-api-openapi.yml
- filename: listmonk-templates-api-openapi.yml
  format: yaml
  label: listmonk Templates API
  slug: listmonk-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-templates-api-openapi.yml
- filename: listmonk-transactional-api-openapi.yml
  format: yaml
  label: listmonk Transactional API
  slug: listmonk-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-transactional-api-openapi.yml
- filename: listmonk-admin-api-openapi.yml
  format: yaml
  label: listmonk Admin API
  slug: listmonk-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-admin-api-openapi.yml
- filename: listmonk-logs-api-openapi.yml
  format: yaml
  label: listmonk Logs API
  slug: listmonk-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-logs-api-openapi.yml
- filename: listmonk-maintenance-api-openapi.yml
  format: yaml
  label: listmonk Maintenance API
  slug: listmonk-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-maintenance-api-openapi.yml
- filename: listmonk-miscellaneous-api-openapi.yml
  format: yaml
  label: listmonk Miscellaneous API
  slug: listmonk-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-miscellaneous-api-openapi.yml
- filename: listmonk-public-api-openapi.yml
  format: yaml
  label: listmonk Public API
  slug: listmonk-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-public-api-openapi.yml
- filename: listmonk-settings-api-openapi.yml
  format: yaml
  label: listmonk Settings API
  slug: listmonk-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-settings-api-openapi.yml
auth_types:
- http
- apiKey
description: 'listmonk''s API authentication is deliberately simple and entirely operator-issued: there is no vendor, no key-issuing console and no token service. An administrator creates an "API user" in the admin UI, listmonk generates a secret token for it, and every call carries that api_user:token pair either as HTTP Basic credentials or in an `Authorization: token` header. What listmonk does have, and what most self-hosted tools of its size do not, is a real authorization layer behind that: 33 named permissions grouped into User roles, plus per-list read/write grants grouped into List roles, enforced on API calls and not merely in the UI. OIDC exists but is for administrator sign-in only — no OIDC or OAuth token is accepted on /api/*.'
kind: authentication
layout: security
method: searched
name: Listmonk Authentication
name_suffix: Authentication
oauth_flows: []
overview: listmonk secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: listmonk
provider_slug: listmonk
scheme_count: 2
schemes:
- description: HTTP Basic auth using an API user name and token (api_user:token).
  example: curl -u "api_user:token" http://localhost:9000/api/lists
  name: BasicAuth
  scheme: basic
  sources:
  - https://listmonk.app/docs/apis/apis/
  - openapi/listmonk-subscribers-api-openapi.yml
  type: http
- description: 'Authorization header in the form: token api_user:token.'
  example: 'curl -H "Authorization: token api_user:token" http://localhost:9000/api/lists'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - https://listmonk.app/docs/apis/apis/
  - openapi/listmonk-subscribers-api-openapi.yml
  type: apiKey
slug: listmonk-authentication
source_filename: listmonk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://listmonk.app/docs/apis/apis/ ,\n  https://listmonk.app/docs/roles-and-permissions/ ,\n  https://listmonk.app/docs/oidc/ , plus the securitySchemes in\n  openapi/listmonk-*-openapi.yml and a live probe of\n  https://demo.listmonk.app/api/health on 2026-08-13\ndocs: https://listmonk.app/docs/apis/apis/\ndescription: >-\n  listmonk's API authentication is deliberately simple and entirely\n  operator-issued: there is no vendor, no key-issuing console and no token\n  service. An administrator creates an \"API user\" in the admin UI, listmonk\n  generates a secret token for it, and every call carries that api_user:token\n  pair either as HTTP Basic credentials or in an `Authorization: token` header.\n  What listmonk does have, and what most self-hosted tools of its size do not, is\n  a real authorization layer behind that: 33 named permissions grouped into User\n  roles, plus per-list read/write grants grouped into\
  \ List roles, enforced on API\n  calls and not merely in the UI. OIDC exists but is for administrator sign-in\n  only — no OIDC or OAuth token is accepted on /api/*.\nsummary:\n  types:\n    - http\n    - apiKey\n  api_key_in:\n    - header\n  oauth2: false\n  openid_connect: admin-sso-only\n  mtls: false\n  scopes: rbac-permissions\n  scope_count: 33\nschemes:\n  - name: BasicAuth\n    type: http\n    scheme: basic\n    description: HTTP Basic auth using an API user name and token (api_user:token).\n    example: curl -u \"api_user:token\" http://localhost:9000/api/lists\n    sources:\n      - https://listmonk.app/docs/apis/apis/\n      - openapi/listmonk-subscribers-api-openapi.yml\n  - name: TokenAuth\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: 'Authorization header in the form: token api_user:token.'\n    example: 'curl -H \"Authorization: token api_user:token\" http://localhost:9000/api/lists'\n    sources:\n      - https://listmonk.app/docs/apis/apis/\n\
  \      - openapi/listmonk-subscribers-api-openapi.yml\ncredentials:\n  issuance: >-\n    Created by an administrator under Admin -> Users. A user account is either a\n    regular user or an API user; API users get an automatically generated secret\n    token instead of a password and exist specifically for programmatic access.\n  rotation_policy: null\n  expiry: null\n  note: >-\n    No documented token rotation, expiry, or last-used telemetry. Rotation means\n    regenerating the API user's token in the admin UI.\nfailure_behaviour:\n  unauthenticated_status: 403\n  body: '{\"message\":\"invalid session\"}'\n  evidence: >-\n    Probed https://demo.listmonk.app/api/health on 2026-08-13 with no\n    credentials — HTTP 403, not 401, and no WWW-Authenticate challenge. Clients\n    branching on 401 will miss listmonk's auth failures.\nunauthenticated_surface:\n  - operation: getPublicLists\n    path: GET /api/public/lists\n  - operation: handlePublicSubscription\n    path: POST /api/public/subscription\n\
  unauthenticated_surface_note: >-\n  The public opt-in surface, gated by the `app.enable_public_subscription_page`\n  setting. Everything else requires credentials.\nadmin_authentication:\n  password: true\n  totp_2fa: true\n  totp_since: v6.0.0\n  password_reset: e-mail based \"Forgot password\" flow, added in v6.0.0\n  oidc:\n    supported: true\n    docs: https://listmonk.app/docs/oidc/\n    scope: Administrator sign-in to the listmonk admin UI only.\n    auto_provisioning: >-\n      Since v5.1.0 listmonk can auto-create OIDC users and assign default user\n      and list roles.\n    note: >-\n      NOT an API authorization model. An OIDC access token cannot be presented to\n      /api/*; API callers must use an API user's token.\n  captcha:\n    current: ALTCHA (self-contained proof-of-work)\n    deprecated: hCaptcha (deprecated in v5.1.0)\nauthorization:\n  model: rbac\n  docs: https://listmonk.app/docs/roles-and-permissions/\n  precedence: >-\n    `lists:get_all` and `lists:manage_all`\
  \ in a User role supersede and override\n    any list-specific permission granted in a List role.\n  user_role_permissions:\n    - group: lists\n      permissions:\n        - name: lists:get_all\n          description: Get details of all lists.\n        - name: lists:manage_all\n          description: Create, update, and delete all lists.\n    - group: subscribers\n      permissions:\n        - name: subscribers:get\n          description: Get individual subscriber details.\n        - name: subscribers:get_all\n          description: Get all subscribers and their details.\n        - name: subscribers:manage\n          description: Add, update, and delete subscribers.\n        - name: subscribers:import\n          description: Import subscribers from external files.\n        - name: subscribers:sql_query\n          description: >-\n            Run raw SQL queries on subscriber data. listmonk flags this as high\n            risk: read-only on table data, but it supersedes individual list\
  \ and\n            subscriber permissions and can reach Postgres system features. Grant\n            only to trusted users.\n          risk: high\n        - name: tx:send\n          description: Send transactional messages to subscribers.\n    - group: campaigns\n      permissions:\n        - name: campaigns:get\n          description: Get and view campaigns belonging to permitted lists.\n        - name: campaigns:get_all\n          description: Get and view campaigns across all lists.\n        - name: campaigns:get_analytics\n          description: Access campaign performance metrics.\n        - name: campaigns:manage\n          description: Create, update, and delete campaigns belonging to permitted lists.\n        - name: campaigns:manage_all\n          description: Create, update, and delete campaigns across all lists.\n        - name: campaigns:send\n          description: >-\n            Start, schedule, pause, resume, and cancel campaigns. Independent of\n            manage permissions\
  \ — required to send even with campaigns:manage_all.\n          since: v6.1.0\n    - group: bounces\n      permissions:\n        - name: bounces:get\n          description: Get email bounce records.\n        - name: bounces:manage\n          description: Process and handle bounced emails.\n        - name: webhooks:post_bounce\n          description: Receive bounce notifications via webhook (POST /webhooks/bounce).\n    - group: media\n      permissions:\n        - name: media:get\n          description: Get uploaded media files.\n        - name: media:manage\n          description: Upload, update, and delete media.\n    - group: templates\n      permissions:\n        - name: templates:get\n          description: Get email templates.\n        - name: templates:manage\n          description: Create, update, and delete templates.\n    - group: users\n      permissions:\n        - name: users:get\n          description: Get system user accounts.\n        - name: users:manage\n          description:\
  \ >-\n            Create, update, and delete user accounts. Allows creation of users\n            with any role including Super Admin — Super Admin level only.\n          risk: high\n        - name: roles:get\n          description: Get user roles and permissions.\n        - name: roles:manage\n          description: Create and modify user roles.\n    - group: settings\n      permissions:\n        - name: settings:get\n          description: Get system settings.\n        - name: settings:manage\n          description: Modify system configuration.\n        - name: settings:maintain\n          description: Perform system maintenance tasks.\n  list_roles:\n    description: >-\n      Per-list view (read) or manage (update) grants, composed into a List role\n      and attached to a user. Only the lists named in the role are accessible,\n      through the admin UI and through the API alike.\nscopes_artifact: null\nscopes_note: >-\n  No scopes/ artifact is emitted. listmonk has no OAuth surface,\
  \ so there are no\n  OAuth scopes; the permission model above is listmonk RBAC and is recorded here\n  rather than dressed up as scopes it is not.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/authentication/listmonk-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Email
- Newsletter
- Mailing List
- Marketing
- Transactional Email
- Campaigns
- Subscribers
- Bounce Handling
- Open-Source
- Self-Hosted
- Go
- PostgreSQL
---
