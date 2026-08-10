---
api_key_in:
- query
api_specs:
- filename: hey-api-get-api-openapi.yml
  format: yaml
  label: Hey API Get API
  slug: hey-api-get-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hey-api/refs/heads/main/openapi/hey-api-get-api-openapi.yml
- filename: hey-api-hey-api-api-openapi.yml
  format: yaml
  label: Hey API Hey API API
  slug: hey-api-hey-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hey-api/refs/heads/main/openapi/hey-api-hey-api-api-openapi.yml
- filename: hey-api-internal-api-openapi.yml
  format: yaml
  label: Hey API Internal API
  slug: hey-api-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hey-api/refs/heads/main/openapi/hey-api-internal-api-openapi.yml
- filename: hey-api-organizations-api-openapi.yml
  format: yaml
  label: Hey API Organizations API
  slug: hey-api-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hey-api/refs/heads/main/openapi/hey-api-organizations-api-openapi.yml
- filename: hey-api-specifications-api-openapi.yml
  format: yaml
  label: Hey API Specifications API
  slug: hey-api-specifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hey-api/refs/heads/main/openapi/hey-api-specifications-api-openapi.yml
- filename: hey-api-users-api-openapi.yml
  format: yaml
  label: Hey API Users API
  slug: hey-api-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hey-api/refs/heads/main/openapi/hey-api-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Hey Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hey API secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hey API
provider_slug: hey-api
scheme_count: 2
schemes:
- applies_to:
  - POST /v1/specifications
  - GET /v1/get/{organization_slug}/{project_slug}
  description: 'Hey API Platform API key, sent as `Authorization: Bearer <api_key>`. Two kinds exist and they are NOT interchangeable — see key_types below.'
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/hey-api-platform-openapi.json
  type: http
- applies_to: 33 of 38 operations (every /v1/organizations, /v1/users and /v1/internal path)
  bearerFormat: JWT
  description: Clerk-issued session JWT. This is the browser/console credential — it secures every organization, project, member, api-key, webhook, waitlist and user management operation on the platform API.
  identity_provider:
    evidence: '`Clerk JWT token` securityScheme description in the spec; the `clerk_user_id` field on the User schema; and the `x-clerk-auth-reason: session-token-and-uat-missing` response header observed on an anonymous GET to api.heyapi.dev.'
    name: Clerk
  name: Clerk
  scheme: bearer
  sources:
  - openapi/hey-api-platform-openapi.json
  type: http
slug: hey-api-authentication
source_filename: hey-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: openapi/hey-api-platform-openapi.json\ndocs: https://heyapi.dev/docs/openapi/typescript/integrations\nsummary:\n  types:\n    - http\n  http_schemes:\n    - bearer\n  api_key_in:\n    - query\n  oauth2_flows: []\n  identity_provider: Clerk\nschemes:\n  - name: ApiKey\n    type: http\n    scheme: bearer\n    description: >-\n      Hey API Platform API key, sent as `Authorization: Bearer <api_key>`.\n      Two kinds exist and they are NOT interchangeable — see key_types below.\n    sources:\n      - openapi/hey-api-platform-openapi.json\n    applies_to:\n      - POST /v1/specifications\n      - GET /v1/get/{organization_slug}/{project_slug}\n  - name: Clerk\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Clerk-issued session JWT. This is the browser/console credential — it\n      secures every organization, project, member, api-key, webhook, waitlist\n      and user management operation\
  \ on the platform API.\n    sources:\n      - openapi/hey-api-platform-openapi.json\n    identity_provider:\n      name: Clerk\n      evidence: >-\n        `Clerk JWT token` securityScheme description in the spec; the\n        `clerk_user_id` field on the User schema; and the\n        `x-clerk-auth-reason: session-token-and-uat-missing` response header\n        observed on an anonymous GET to api.heyapi.dev.\n    applies_to: 33 of 38 operations (every /v1/organizations, /v1/users and /v1/internal path)\nalternate_transport:\n  - name: api_key query parameter\n    in: query\n    parameter: api_key\n    description: >-\n      The spec-download endpoint additionally accepts the key as a query\n      parameter so any codegen CLI can consume the URL directly, e.g.\n      https://get.heyapi.dev/foo/bar?api_key=<my_api_key>\n    documented_at: https://heyapi.dev/docs/openapi/typescript/integrations\n    caution: >-\n      Query-parameter credentials land in proxy and CDN access logs and in\n\
  \      shell history. Prefer the Authorization header where the toolchain allows.\nkey_types:\n  - name: project API key\n    scope: one project\n    issued_at: app.heyapi.dev > project > Integrations > APIs\n    can_upload: true\n    intended_for: CI workflows (the hey-api/upload-openapi-spec GitHub Action reads it from $API_KEY)\n  - name: personal API key\n    scope: the user's accessible projects\n    issued_at: https://app.heyapi.dev/settings/user/apis\n    can_upload: false\n    intended_for: local development / pulling specs\n    evidence: 'Docs: \"Personal API keys can''t be used to upload specifications.\"'\nanonymous_access:\n  - operation: GET /\n    note: Unauthenticated liveness response — \"Hey API Backend v1.0.0\".\n  - operation: GET /v1/get/{organization_slug}/{project_slug}\n    note: >-\n      The spec declares an empty security requirement `{}` alongside ApiKey and\n      Clerk, i.e. anonymous access is permitted for PUBLIC projects. Projects\n      are private by default;\
  \ hey-api/backend is public, which is how this\n      repo harvested the platform OpenAPI without credentials.\nkey_lifecycle:\n  create: POST /v1/organizations/{organization_slug}/projects/{project_slug}/api-keys\n  list: GET /v1/organizations/{organization_slug}/projects/{project_slug}/api-keys\n  rotate_or_update: POST /v1/organizations/{organization_slug}/projects/{project_slug}/api-keys/{api_key_id}\n  revoke: DELETE /v1/organizations/{organization_slug}/projects/{project_slug}/api-keys/{api_key_id}\n  personal_keys: /v1/users/{user_id}/api-keys\n  last_used_tracking: 'ApiKeyConcealed.last_used_at is returned on every key listing'\n  value_disclosure: >-\n    The full key value is only present on the `ApiKey` schema (returned at\n    creation); listings return `ApiKeyConcealed`, which omits `value`.\noauth2: false\nscopes: none\nnotes: >-\n  No OAuth 2.0 and no OpenID Connect provider metadata is exposed by Hey API\n  itself — /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server\
  \ both 404 on every host. Console\n  identity is delegated to Clerk; API-to-API identity is a bearer API key.\n  There is therefore no scopes/ artifact for this provider.\nx-evidence:\n  fetched: '2026-08-06'\n  spec_url: https://api.heyapi.dev/v1/get/hey-api/backend\n  spec_http_status: 200\n  docs_url: https://heyapi.dev/docs/openapi/typescript/integrations\n  docs_http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hey-api/refs/heads/main/authentication/hey-api-authentication.yml
summary_line: http · 2 schemes
tags:
- Code Generation
- Developer Tools
- OpenAPI
- SDKs
- TypeScript
- Python
- API Design
- Specifications
- Registry
- Open Source
---
