---
api_key_in:
- header
api_specs:
- filename: 0g-labs-account-api-openapi.yml
  format: yaml
  label: 0G Labs Account API
  slug: 0g-labs-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0g-labs/refs/heads/main/openapi/0g-labs-account-api-openapi.yml
- filename: 0g-labs-api-key-api-openapi.yml
  format: yaml
  label: 0G Labs API Key API
  slug: 0g-labs-api-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0g-labs/refs/heads/main/openapi/0g-labs-api-key-api-openapi.yml
- filename: 0g-labs-inference-api-openapi.yml
  format: yaml
  label: 0G Labs Inference API
  slug: 0g-labs-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0g-labs/refs/heads/main/openapi/0g-labs-inference-api-openapi.yml
- filename: 0g-labs-models-api-openapi.yml
  format: yaml
  label: 0G Labs Models API
  slug: 0g-labs-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0g-labs/refs/heads/main/openapi/0g-labs-models-api-openapi.yml
- filename: 0g-labs-provider-api-openapi.yml
  format: yaml
  label: 0G Labs Provider API
  slug: 0g-labs-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0g-labs/refs/heads/main/openapi/0g-labs-provider-api-openapi.yml
- filename: 0g-labs-service-types-api-openapi.yml
  format: yaml
  label: 0G Labs Service Types API
  slug: 0g-labs-service-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0g-labs/refs/heads/main/openapi/0g-labs-service-types-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: 0G Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: 0G Labs secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 0G Labs
provider_slug: 0g-labs
scheme_count: 2
schemes:
- description: 'API key for inference, file upload, and async image endpoints. Format: "Bearer sk-..."'
  format: Bearer sk-...
  in: header
  issuance: Dashboard > API Keys. The full secret is shown once on creation; the dashboard stores only a hash. Keys are labelled, listed with created-at and last-used, and revocable instantly — a revoked key returns 401 api_key_revoked on its next call.
  issued_at: https://pc.0g.ai
  name: ApiKeyAuth
  parameter: Authorization
  prefix: sk-
  purpose: Call inference endpoints (/v1/chat/completions, /v1/messages, /v1/images/*, /v1/audio/transcriptions, /v1/videos, /v1/routing/preview). Billed against the account's on-chain deposit.
  scoped: false
  sources:
  - openapi/0g-labs-router-openapi.yml
  type: apiKey
- audit_fields:
  - last_used_at
  - last_source_ip
  audit_note: Updated on every successful mk- request, coalesced to at most one write per key per 60s. IPv4-mapped IPv6 addresses are normalized to dotted-quad. sk- keys do not record these — their audit signal is usage/billing.
  description: 'Management key for account read and API key management. Capabilities are scope-limited per key (account:read, keys:read, keys:create, keys:manage). Format: "Bearer mk-..."'
  format: Bearer mk-...
  in: header
  issuance: Settings > Management Keys. Each key carries an explicit scope allowlist. Keys do not expire.
  issued_at: https://pc.0g.ai
  name: ManagementKeyAuth
  parameter: Authorization
  prefix: mk-
  presets:
  - name: Read-only
    scopes:
    - account:read
    - keys:read
  - name: Key Manager
    scopes:
    - keys:read
    - keys:manage
  - name: Full Admin
    scopes:
    - account:read
    - keys:read
    - keys:create
    - keys:manage
  purpose: Administer the account — read balance/usage/history and list, create, edit or revoke API keys. Not billed. Cannot call inference.
  scoped: true
  scopes:
  - description: Read balance, usage and per-request history (GET /v1/account/*).
    name: account:read
  - description: List API keys (GET /v1/api-keys).
    name: keys:read
  - description: Create API keys (POST /v1/api-keys).
    name: keys:create
  - description: Edit or revoke API keys (PATCH / DELETE /v1/api-keys/{keyId}).
    name: keys:manage
  sources:
  - openapi/0g-labs-router-openapi.yml
  type: apiKey
slug: 0g-labs-authentication
source_filename: 0g-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: openapi/0g-labs-router-openapi.yml\ndocs: https://docs.0g.ai/developer-hub/building-on-0g/compute-network/router/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    No OAuth flow, no wallet signature per request, no session tokens on the Router. Two\n    prefixed bearer credentials do everything. A separate wallet JWT (sign-in session at\n    pc.0g.ai) is required for management-key administration and is not issuable as a key.\n    The 0G Compute \"Direct\" path is different: it has no API key at all — the caller's wallet\n    signs each request against a per-provider sub-account.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: Bearer sk-...\n  prefix: sk-\n  purpose: >-\n    Call inference endpoints (/v1/chat/completions, /v1/messages, /v1/images/*,\n    /v1/audio/transcriptions, /v1/videos, /v1/routing/preview). Billed\
  \ against the account's\n    on-chain deposit.\n  description: 'API key for inference, file upload, and async image endpoints. Format: \"Bearer sk-...\"'\n  issued_at: https://pc.0g.ai\n  issuance: >-\n    Dashboard > API Keys. The full secret is shown once on creation; the dashboard stores only a\n    hash. Keys are labelled, listed with created-at and last-used, and revocable instantly — a\n    revoked key returns 401 api_key_revoked on its next call.\n  scoped: false\n  sources:\n  - openapi/0g-labs-router-openapi.yml\n- name: ManagementKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: Bearer mk-...\n  prefix: mk-\n  purpose: >-\n    Administer the account — read balance/usage/history and list, create, edit or revoke API\n    keys. Not billed. Cannot call inference.\n  description: >-\n    Management key for account read and API key management. Capabilities are scope-limited per\n    key (account:read, keys:read, keys:create, keys:manage). Format: \"Bearer\
  \ mk-...\"\n  issued_at: https://pc.0g.ai\n  issuance: Settings > Management Keys. Each key carries an explicit scope allowlist. Keys do not expire.\n  scoped: true\n  scopes:\n  - name: account:read\n    description: Read balance, usage and per-request history (GET /v1/account/*).\n  - name: keys:read\n    description: List API keys (GET /v1/api-keys).\n  - name: keys:create\n    description: Create API keys (POST /v1/api-keys).\n  - name: keys:manage\n    description: Edit or revoke API keys (PATCH / DELETE /v1/api-keys/{keyId}).\n  presets:\n  - name: Read-only\n    scopes: [account:read, keys:read]\n  - name: Key Manager\n    scopes: [keys:read, keys:manage]\n  - name: Full Admin\n    scopes: [account:read, keys:read, keys:create, keys:manage]\n  audit_fields:\n  - last_used_at\n  - last_source_ip\n  audit_note: >-\n    Updated on every successful mk- request, coalesced to at most one write per key per 60s.\n    IPv4-mapped IPv6 addresses are normalized to dotted-quad. sk- keys do\
  \ not record these —\n    their audit signal is usage/billing.\n  sources:\n  - openapi/0g-labs-router-openapi.yml\npermission_matrix:\n- scenario: Run inference\n  endpoint: POST /v1/chat/completions (and other inference endpoints)\n  api_key: allowed\n  management_key: denied\n- scenario: Read balance / usage / history\n  endpoint: GET /v1/account/*\n  api_key: denied\n  management_key: allowed\n  required_scope: account:read\n- scenario: List API keys\n  endpoint: GET /v1/api-keys\n  api_key: denied\n  management_key: allowed\n  required_scope: keys:read\n- scenario: Create API key\n  endpoint: POST /v1/api-keys\n  api_key: denied\n  management_key: allowed\n  required_scope: keys:create\n- scenario: Edit / revoke API key\n  endpoint: PATCH or DELETE /v1/api-keys/{keyId}\n  api_key: denied\n  management_key: allowed\n  required_scope: keys:manage\n- scenario: Manage management keys\n  endpoint: ANY /v1/management-keys/*\n  api_key: denied\n  management_key: denied\n  required: wallet\
  \ JWT (sign-in session) only\n  rationale: >-\n    A leaked mk- cannot mint replacements for itself. keys:manage and keys:create are also\n    deliberately split so an audit integration can revoke a compromised key without being able\n    to issue a new one.\nunauthenticated_endpoints:\n- GET /v1/models\n- GET /v1/providers\n- GET /v1/service-types\nguidance:\n- Never ship either key to a browser — proxy client requests through your own backend.\n- One key per deployment so a revocation is scoped to one service.\n- Least privilege for mk-; rotate by issuing a replacement and revoking the old key.\nbreaking_change:\n  observed: '2026-08-05'\n  detail: >-\n    sk- keys no longer have access to /v1/account/* (balance, usage, history). Existing\n    dashboard/billing code must move to an mk- key with the account:read scope.\n  source: https://docs.0g.ai/developer-hub/building-on-0g/compute-network/router/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/0g-labs/refs/heads/main/authentication/0g-labs-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Artificial Intelligence
- AI Inference
- LLM
- GPU Compute
- Decentralized Compute
- Blockchain
- Web3
- EVM
- Decentralized Storage
- Data Availability
- OpenAI-Compatible
- Trusted Execution Environment
- agent-native
- Crypto Infrastructure
---
