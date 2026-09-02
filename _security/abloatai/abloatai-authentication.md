---
api_key_in:
- header
api_specs:
- filename: abloatai-branches-api-openapi.yml
  format: yaml
  label: Ablo Branches API
  slug: ablo-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-branches-api-openapi.yml
- filename: abloatai-claims-api-openapi.yml
  format: yaml
  label: Ablo Claims API
  slug: ablo-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-claims-api-openapi.yml
- filename: abloatai-commits-api-openapi.yml
  format: yaml
  label: Ablo Commits API
  slug: ablo-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-commits-api-openapi.yml
- filename: abloatai-credentials-api-openapi.yml
  format: yaml
  label: Ablo Credentials API
  slug: ablo-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-credentials-api-openapi.yml
- filename: abloatai-logs-api-openapi.yml
  format: yaml
  label: Ablo Logs API
  slug: ablo-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-logs-api-openapi.yml
- filename: abloatai-models-api-openapi.yml
  format: yaml
  label: Ablo Models API
  slug: ablo-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-models-api-openapi.yml
- filename: abloatai-schema-api-openapi.yml
  format: yaml
  label: Ablo Schema API
  slug: ablo-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-schema-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Abloatai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ablo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ablo
provider_slug: abloatai
scheme_count: 1
schemes:
- applied: global (every operation in the spec)
  description: Your Ablo API key (sk_… / rk_…).
  header: 'Authorization: Bearer <key>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/abloatai-api-openapi.yml
  type: http
slug: abloatai-authentication
source_filename: abloatai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: searched\nsource: https://docs.abloatai.com/api-keys\ndocs: https://docs.abloatai.com/api-keys\nderived_from: openapi/abloatai-api-openapi.yml\nnote: >-\n  The OpenAPI declares a single scheme — HTTP bearer — which understates the model considerably.\n  Ablo's real credential system is a prefix-typed capability class carried in the bearer token,\n  plus an optional scope set, plus an immutable server-side branch binding. All three are\n  authority boundaries and only the first is visible in the spec. There is no OAuth 2.0 and no\n  OIDC surface: /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n  both 404 on the API host, so scopes/ is deliberately not emitted (the scope strings below are\n  key grants, not OAuth scopes).\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  openid_connect: false\n  mtls: false\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme:\
  \ bearer\n    header: 'Authorization: Bearer <key>'\n    description: Your Ablo API key (sk_… / rk_…).\n    applied: global (every operation in the spec)\n    sources: [openapi/abloatai-api-openapi.yml]\ncredential_classes:\n  - prefix: sk_\n    name: trusted runtime secret\n    use: server, worker or agent that can hold a secret; default env var ABLO_API_KEY\n    browser_safe: false\n    note: 'With an empty scope set an sk_ key carries full org authority. Blocked client-side — using one from a browser raises browser_apikey_blocked.'\n  - prefix: rk_\n    name: restricted / delegated runtime\n    use: another runtime that needs only a delegated scope\n    browser_safe: false\n  - prefix: pk_\n    name: publishable browser key\n    use: browser bundle; read-only access to the org data plane\n    browser_safe: true\n    write: false\n  - prefix: ek_\n    name: ephemeral user session\n    use: short-lived, minted server-side and held in browser memory\n    browser_safe: true\n    minted_by:\
  \ 'POST /v1/ephemeral_keys (mintEphemeralKey) or server.sessions.create()'\n  - prefix: mk_\n    name: project and branch management\n    use: CLI / CI management credential; the only class that can carry management scopes\n    browser_safe: false\nlegacy_spellings:\n  - 'sk_live_… / sk_test_… / rk_live_… continue to authenticate during migration'\n  - \"The live/test segment is a legacy hint only, not the source of truth; the persisted branch binding controls the key.\"\nscopes:\n  model: key-grant scopes (NOT OAuth scopes) — least privilege; an empty scope set on an sk_ key means full org authority\n  docs: https://docs.abloatai.com/api-keys#scopes\n  grants:\n    - {scope: 'schema:push', description: 'Author the schema artifact on the key''s bound plane (ablo push, ablo dev).'}\n    - {scope: 'project:manage', description: 'List, create and rename projects.', classes: [mk_]}\n    - {scope: 'branch:manage', description: 'List, create and delete child branches and mint their temporary\
  \ credentials.', classes: [mk_]}\n    - {scope: 'organization:act-as', description: 'Cross-organization authority to mint a short-lived user session into a customer organization. Follows the Stripe Connect shape; the resulting session is still bounded by its can grant and expiry.'}\n  session_grants:\n    model: 'Per-session typed can grant, e.g. can: { records: [read, update] } — model/verb scoped, applied when minting an ek_ or rk_.'\nauthority_axes:\n  - axis: capability class\n    carried_by: key prefix\n  - axis: scope set\n    carried_by: server-side key row\n  - axis: branch binding\n    carried_by: immutable server-side binding\n    note: 'A temporary child-branch key can act only inside that child; it cannot manage siblings or gain root authority even with no scope strings.'\njwt:\n  supported: true\n  note: >-\n    The error registry documents a full third-party JWT path (jwt_issuer_untrusted,\n    jwt_audience_mismatch, jwt_missing_organization, jwt_org_membership_denied, issuer_register_forbidden),\n\
  \    so a customer's own IdP can be registered as a trusted issuer. This is not declared in the OpenAPI.\n  source: https://docs.abloatai.com/errors\ncredential_hygiene:\n  - 'A mint returns plaintext exactly once; only a hash is retained, so no API or MCP tool can hand a key back later.'\n  - 'Rotation: POST /v1/capabilities/{id}/rotate (rotateCapability) mints a replacement keeping the grant.'\n  - 'Revocation: DELETE /v1/capabilities/{id} (revokeCapability).'\nfailure_signalling:\n  header: X-Auth-Failure\n  cors_exposed: true\n  note: 'The specific auth failure code is echoed on a CORS-exposed response header, so a browser client can distinguish apikey_invalid from auth_no_credentials without reading the body.'\n  observed:\n    - {probe: 'GET https://api.abloatai.com/api/v1/schema (no credential)', http_status: 401, x_auth_failure: auth_no_credentials}\n    - {probe: 'GET https://api.abloatai.com/api/v1/schema (bogus bearer)', http_status: 401, x_auth_failure: apikey_invalid}\nx-evidence:\n\
  \  - {url: 'https://docs.abloatai.com/api-keys', http_status: 200}\n  - {url: 'https://api.abloatai.com/.well-known/openid-configuration', http_status: 404}\n  - {url: 'https://api.abloatai.com/.well-known/oauth-authorization-server', http_status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/authentication/abloatai-authentication.yml
summary_line: http · 1 scheme
tags:
- Agent Infrastructure
- multi-agent-coordination
- concurrency-control
- State Management
- Database
- Postgres
- real-time-sync
- MCP
- Developer Tools
- backend-infrastructure
---
