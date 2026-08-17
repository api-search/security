---
api_key_in:
- header
api_specs:
- filename: publer-accounts-api-openapi.yml
  format: yaml
  label: Publer Accounts API
  slug: publer-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-accounts-api-openapi.yml
- filename: publer-analytics-api-openapi.yml
  format: yaml
  label: Publer Analytics API
  slug: publer-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-analytics-api-openapi.yml
- filename: publer-competitors-api-openapi.yml
  format: yaml
  label: Publer Competitors API
  slug: publer-competitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-competitors-api-openapi.yml
- filename: publer-jobs-api-openapi.yml
  format: yaml
  label: Publer Jobs API
  slug: publer-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-jobs-api-openapi.yml
- filename: publer-media-api-openapi.yml
  format: yaml
  label: Publer Media API
  slug: publer-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-media-api-openapi.yml
- filename: publer-posts-api-openapi.yml
  format: yaml
  label: Publer Posts API
  slug: publer-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-posts-api-openapi.yml
- filename: publer-users-api-openapi.yml
  format: yaml
  label: Publer Users API
  slug: publer-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-users-api-openapi.yml
- filename: publer-workspaces-api-openapi.yml
  format: yaml
  label: Publer Workspaces API
  slug: publer-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-workspaces-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Publer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Publer secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Publer
provider_slug: publer
scheme_count: 2
schemes:
- description: 'API key passed as `Authorization: Bearer-API YOUR_API_KEY`. The auth-scheme token is `Bearer-API`, NOT the RFC 6750 `Bearer` — off-the-shelf bearer clients and generated SDKs will fail with 401 unless the prefix is customized. This is the single most common integration mistake on this API.'
  format: Bearer-API YOUR_API_KEY
  in: header
  name: BearerApiAuth
  parameter: Authorization
  sources:
  - openapi/_original/publer-openapi.yml
  - https://publer.com/docs/getting-started/authentication.md
  type: apiKey
- description: Workspace scoping header, required on most endpoints (accounts, media, posts, analytics, competitors, jobs). Obtained from GET /workspaces. Omitting it returns 403 Forbidden, not 401 — a distinction that misleads clients into re-checking their key.
  in: header
  name: workspace_id
  note: Declared as a securityScheme in some of Publer's per-page OpenAPI blocks and as a required header PARAMETER in others — the specification is not internally consistent about which it is.
  parameter: Publer-Workspace-Id
  sources:
  - openapi/_original/publer-openapi.yml
  - https://publer.com/docs/api-reference/workspaces.md
  type: apiKey
slug: publer-authentication
source_filename: publer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://publer.com/docs/getting-started/authentication.md\nsource: >-\n  https://publer.com/docs/getting-started/authentication.md,\n  https://publer.com/docs/api-reference/introduction.md,\n  https://publer.com/help/en/article/how-to-access-the-publer-api-1w08edo/ —\n  cross-checked against openapi/_original/publer-openapi.yml\nprovider: Publer\nproviderId: publer\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  scoped: true\n  note: >-\n    API key only. Publer runs no OAuth 2.0 or OIDC authorization server, and\n    serves no /.well-known/oauth-authorization-server or\n    /.well-known/openid-configuration (probed 2026-08-13 — publer.com returns a\n    Framer SPA HTML shell, app.publer.com returns 410). Keys are long-lived and\n    user-scoped; the scope set is chosen at creation time.\nschemes:\n- name: BearerApiAuth\n  type: apiKey\n  in: header\n  parameter:\
  \ Authorization\n  format: 'Bearer-API YOUR_API_KEY'\n  description: >-\n    API key passed as `Authorization: Bearer-API YOUR_API_KEY`. The auth-scheme\n    token is `Bearer-API`, NOT the RFC 6750 `Bearer` — off-the-shelf bearer\n    clients and generated SDKs will fail with 401 unless the prefix is\n    customized. This is the single most common integration mistake on this API.\n  sources:\n  - openapi/_original/publer-openapi.yml\n  - https://publer.com/docs/getting-started/authentication.md\n- name: workspace_id\n  type: apiKey\n  in: header\n  parameter: Publer-Workspace-Id\n  description: >-\n    Workspace scoping header, required on most endpoints (accounts, media,\n    posts, analytics, competitors, jobs). Obtained from GET /workspaces.\n    Omitting it returns 403 Forbidden, not 401 — a distinction that misleads\n    clients into re-checking their key.\n  sources:\n  - openapi/_original/publer-openapi.yml\n  - https://publer.com/docs/api-reference/workspaces.md\n  note: >-\n \
  \   Declared as a securityScheme in some of Publer's per-page OpenAPI blocks and\n    as a required header PARAMETER in others — the specification is not\n    internally consistent about which it is.\nkey_management:\n  issuance: >-\n    Self-service in the Publer app — Settings -> Access & Login -> API Keys (the\n    help center also documents Settings -> API & Webhooks). Name is required;\n    scopes are selected at creation.\n  visibility: shown once at creation; not retrievable afterwards\n  rotation: >-\n    Manual. Publer recommends rotating every 90-180 days, or after team changes\n    or incidents. Keys cannot be re-scoped — remove and recreate.\n  revocation: self-service removal from the same settings screen\n  expiry: not documented\n  multiple_keys: >-\n    Supported and recommended (separate keys per use case for least privilege),\n    but note the rate limit is applied per USER ACCOUNT across all keys, so\n    splitting keys does not split throughput.\n  self_test: >-\n \
  \   The app provides a \"Try it out\" console that fires test requests against\n    selected endpoints with the new key.\nscopes:\n  supported: true\n  model: per-key permission scopes selected at creation\n  mandatory:\n  - workspaces\n  - accounts\n  optional:\n  - posts\n  - media\n  - analytics\n  see: scopes/publer-scopes.yml\nerrors:\n  '401':\n  - Missing or invalid Authorization header\n  - Key revoked or expired\n  '403':\n  - Insufficient scopes for the endpoint\n  - Missing Publer-Workspace-Id header\n  - Plan entitlement missing (e.g. analytics requires a paying subscription)\n  body: '{\"errors\": [\"Detailed error message\"]}'\n  note: >-\n    403 conflates three unrelated causes and there is no machine-readable code\n    to tell them apart — only the message string.\nentitlement:\n  gated: true\n  requirement: >-\n    Enterprise plan, Business plan in good standing (no failed or locked\n    subscription), or Top Ambassador status.\n  source: https://publer.com/help/en/article/does-publer-have-a-public-api-194nknf/\n\
  transport:\n  https_required: true\n  tls: TLSv1.3 on app.publer.com (probed 2026-08-13)\n  see: security/publer-domain-security.yml\nprovider_guidance:\n- Store keys in environment variables or a secrets vault, never in code.\n- Rotate every 90-180 days or after any team change or incident.\n- Create separate keys per use case (least privilege).\n- Never log a full key; mask all but the last 4 characters.\n- Always use HTTPS.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/authentication/publer-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Social Media
- Scheduling
- Publishing
- Content Management
- Marketing
- Social Media Management
- Analytics
- Agents
- MCP
- Automation
---
