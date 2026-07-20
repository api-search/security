---
api_key_in:
- cookie
- header
api_specs:
- filename: laserdata-core-openapi.json
  format: json
  label: LaserData Cloud Core API
  slug: core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserdata/refs/heads/main/openapi/laserdata-core-openapi.json
- filename: laserdata-audit-openapi.json
  format: json
  label: LaserData Cloud Audit API
  slug: audit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserdata/refs/heads/main/openapi/laserdata-audit-openapi.json
- filename: laserdata-notifier-openapi.json
  format: json
  label: LaserData Cloud Notifier API
  slug: notifier
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserdata/refs/heads/main/openapi/laserdata-notifier-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Laserdata Authentication
name_suffix: Authentication
oauth_flows: []
overview: LaserData secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LaserData
provider_slug: laserdata
scheme_count: 2
schemes:
- description: Tenant API key sent in the ld-api-key request header. Scoped to tenant-level audit reads. Cannot be used on user-scope endpoints (`/audit/users/activity`).
  in: header
  name: ld_api_key
  parameter: ld-api-key
  sources:
  - openapi/laserdata-audit-openapi.json
  - openapi/laserdata-core-openapi.json
  - openapi/laserdata-notifier-openapi.json
  type: apiKey
- description: Browser session cookie issued by POST /account/sign_in on core. Required for user-scope endpoints.
  in: cookie
  name: session_cookie
  parameter: session
  sources:
  - openapi/laserdata-audit-openapi.json
  - openapi/laserdata-core-openapi.json
  - openapi/laserdata-notifier-openapi.json
  type: apiKey
slug: laserdata-authentication
source_filename: laserdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.laserdata.cloud/api/authentication; openapi/laserdata-core-openapi.json, openapi/laserdata-audit-openapi.json,\n  openapi/laserdata-notifier-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\n  oauth2: false\n  oauth2_flows: []\n  primary: ld_api_key\nschemes:\n- name: ld_api_key\n  type: apiKey\n  in: header\n  parameter: ld-api-key\n  description: Tenant API key sent in the ld-api-key request header. Scoped to tenant-level audit reads.\n    Cannot be used on user-scope endpoints (`/audit/users/activity`).\n  sources:\n  - openapi/laserdata-audit-openapi.json\n  - openapi/laserdata-core-openapi.json\n  - openapi/laserdata-notifier-openapi.json\n- name: session_cookie\n  type: apiKey\n  in: cookie\n  parameter: session\n  description: Browser session cookie issued by POST /account/sign_in on core. Required for user-scope\n    endpoints.\n  sources:\n  - openapi/laserdata-audit-openapi.json\n\
  \  - openapi/laserdata-core-openapi.json\n  - openapi/laserdata-notifier-openapi.json\ndocs: https://docs.laserdata.cloud/api/authentication\npermissions_docs: https://docs.laserdata.cloud/organization/roles-permissions\nnotes: Docs are explicit that there are no sessions, cookies or OAuth flows for API access - the session_cookie\n  scheme exists only for Console/user-scope endpoints (/account/*) and tenant creation, and is rejected\n  at runtime on API-key paths. No scopes/ artifact is emitted because LaserData has no OAuth scope surface;\n  authorization is a role/permission model, captured below.\nkey_lifecycle:\n  issued_by: POST /tenants/{tenant_id}/api_keys\n  recoverable: false\n  storage: only the hash is stored server-side - copy the secret immediately after creation\n  format: long-entropy random secret\n  expiry_mandatory: true\n  max_expiry_days: 365\n  expired_behaviour: 401 Unauthorized\n  rotation_guidance: Create a replacement key before expiry and rotate it in CI/CD.\n\
  controls:\n  ip_allowlist:\n    supported: true\n    updatable_in_place: true\n    denied_status: 403\n  rate_limit:\n    scope: per API key\n    status: 429\n    header: retry-after\n  csrf:\n    applies_to: cookie-authenticated mutating endpoints\n    header: X-CSRF-Token\nauthorization:\n  model: role-based, hierarchical\n  docs: https://docs.laserdata.cloud/organization/roles-permissions\n  hierarchy:\n  - tenant\n  - division\n  - environment\n  assignment: Every API key is tied to a role. When creating a key you can assign an existing role or\n    define inline permissions, which auto-creates a dedicated role.\n  scoping:\n  - scope: global\n    description: Three top-level blanket grants - tenant, division and environment - applied across the\n      whole tenant.\n  - scope: per-division\n    description: Override the role's default division permissions for specific divisions.\n  - scope: per-environment\n    description: Within a per-division override, further scope environment\
  \ permissions to specific environments.\n  tenant_permissions:\n  - resource: info\n    read: View tenant information\n    manage: Update tenant information\n  - resource: audit\n    read: View audit logs\n    manage: null\n  - resource: settings\n    read: View tenant settings\n    manage: Update tenant settings\n  - resource: role\n    read: View roles\n    manage: Create, update, and delete roles\n  - resource: member\n    read: View members\n    manage: Invite, update, and remove members\n  - resource: subscription\n    read: View subscription plan\n    manage: Change subscription plan\n  - resource: billing\n    read: View billing and payment\n    manage: Update billing and payment\n  - resource: division\n    read: View divisions\n    manage: Create, update, and delete divisions\n  - resource: api_key\n    read: View API keys\n    manage: Create and delete API keys\n  - resource: notifications\n    read: View notification channels\n    manage: Create, update, and delete notification\
  \ channels\n  example_permission_strings:\n  - member:read\n  - api_key:manage\n  - deployment:manage\n  - deployment:config:read\n  - billing:manage\n  - subscription:manage\nerrors:\n  '401': Key missing, malformed, expired, or revoked.\n  '403': Key valid but missing the required permission, or request from a blocked IP.\n  '404': Resource does not exist or is not visible to this key.\n  '429': Per-key rate limit exceeded; check Retry-After.\n  envelope: errors/laserdata-problem-types.yml\ncli_credentials:\n  keyring: OS keyring (Keychain on macOS, Secret Service on Linux)\n  env:\n  - LD_API_KEY\n  - LD_TENANT_ID\n  guidance: Do not pass --api-key inline; it leaks into shell history.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laserdata/refs/heads/main/authentication/laserdata-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Streaming
- Message Streaming
- Event Streaming
- Data Infrastructure
- Real Time
- Apache Iggy
- Rust
- Cloud Infrastructure
- AI Agents
- Observability
- Company
---
