---
api_key_in:
- header
api_specs:
- filename: tether-api-keys-api-openapi.yml
  format: yaml
  label: Tether API Keys API
  slug: tether-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tether/refs/heads/main/openapi/tether-api-keys-api-openapi.yml
- filename: tether-chains-api-openapi.yml
  format: yaml
  label: Tether Chains API
  slug: tether-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tether/refs/heads/main/openapi/tether-chains-api-openapi.yml
- filename: tether-health-api-openapi.yml
  format: yaml
  label: Tether Health API
  slug: tether-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tether/refs/heads/main/openapi/tether-health-api-openapi.yml
- filename: tether-token-balances-api-openapi.yml
  format: yaml
  label: Tether Token Balances API
  slug: tether-token-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tether/refs/heads/main/openapi/tether-token-balances-api-openapi.yml
- filename: tether-token-transfers-api-openapi.yml
  format: yaml
  label: Tether Token Transfers API
  slug: tether-token-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tether/refs/heads/main/openapi/tether-token-transfers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tether Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tether secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tether
provider_slug: tether
scheme_count: 1
schemes:
- description: API key obtained via the registration form. Include in the X-API-KEY header for all authenticated requests.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/tether-wdk-indexer-openapi-original.yml
  type: apiKey
slug: tether-authentication
source_filename: tether-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: openapi/tether-wdk-indexer-openapi-original.yml\ndocs: https://docs.wdk.tether.io/tools/indexer-api/api-reference\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  x-note: >-\n    Single-scheme provider. No OAuth 2.0, no OpenID Connect, no mutual TLS, no HTTP\n    basic or bearer anywhere in Tether's public API surface — which is why no\n    scopes/ artifact is emitted (there is no scope surface to describe).\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key obtained via the registration form. Include in the X-API-KEY\n    header for all authenticated requests.\n  sources:\n  - openapi/tether-wdk-indexer-openapi-original.yml\nissuance:\n  self_service: true\n  registration_url: https://wdk-api.tether.io/register\n  cost: free\n  api_managed: true\n  operations:\n  - operationId: createApiKey\n    method: POST\n    path: /api/v1/keys\n\
  \    note: Returns the plaintext key ONCE, plus its hashedKey, owner, ttl, label,\n      createdAt and lastActive.\n  - operationId: listApiKeys\n    method: GET\n    path: /api/v1/keys\n    note: >-\n      Also returns the key's own rate-limit budget as `max` and `timeWindow` — the\n      only runtime path to that figure, since no RateLimit-* headers are sent.\n  - operationId: deleteApiKey\n    method: DELETE\n    path: /api/v1/keys/{hashedKey}\n    note: Keys are revoked by HASH, so a revocation script never handles plaintext.\n  expiry:\n    field: ttl\n    unit: milliseconds\n    no_expiry_value: 0\nunauthenticated_operations:\n- operationId: getHealth\n  path: GET /api/v1/health\n- operationId: listChains\n  path: GET /api/v1/chains\nfailure_semantics:\n  '401': Unauthorized — API key EXPIRED.\n  '403': Forbidden — API key MISSING or INVALID.\n  x-note: >-\n    Inverted relative to the common convention, where a missing credential is 401.\n    Rotation logic must trigger on 401,\
  \ not 403.\nsdk_and_agent_auth:\n  x-note: >-\n    The WDK SDK, CLI and MCP Toolkit do not authenticate to Tether at all — they are\n    self-custodial and authenticate to CHAINS with a locally held BIP-39 seed. The\n    only Tether credential in that stack is the optional Indexer API key passed to\n    `useIndexer({ apiKey })`, plus an optional MoonPay key for the fiat modules.\n  secret_handling_published:\n  - Seed phrases stay local; `close()` wipes keys from memory.\n  - Read and write tool sets are separable so an operator can grant read-only access.\n  - Docs mandate a dedicated development wallet with limited funds.\n  - '@tetherto/wdk-secret-manager generates, encrypts and manages seeds.'\n  - '@tetherto/wdk-react-native-secure-storage backs mobile secret storage.'\n  security_model_doc: https://docs.wdk.tether.io/cli/reference/security-model\nx-evidence:\n  fetched: '2026-08-05'\n  urls:\n  - url: https://wdk-api.tether.io/docs/json\n    http_status: 200\n  - url: https://docs.wdk.tether.io/tools/indexer-api/api-reference\n\
  \    http_status: 200\n  - url: https://docs.wdk.tether.io/tools/indexer-api/get-started\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tether/refs/heads/main/authentication/tether-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Stablecoins
- Cryptocurrency
- Blockchain
- Wallets
- Digital Assets
- Payments
- Self-Custody
- Multi-Chain
- Agents
- MCP
- Open Source
---
