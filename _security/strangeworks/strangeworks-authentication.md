---
api_key_in:
- body
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Strangeworks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Strangeworks secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Strangeworks
provider_slug: strangeworks
scheme_count: 3
schemes:
- description: A per-workspace API key issued from the Strangeworks Portal home page. A user who belongs to multiple workspaces has a different key for each. Exchanged for a short-lived JWT — it is not sent on API calls directly.
  exchange_endpoint: POST https://api.strangeworks.com/users/token
  in: body
  issued_at: https://portal.strangeworks.com/
  name: WorkspaceAPIKey
  parameter: key
  sdk_usage: 'import strangeworks as sw

    sw.authenticate(api_key)

    '
  sources:
  - https://docs.strangeworks.com/strangeworks-python
  - pypi:strangeworks-core==0.5.4
  type: apiKey
- description: A product API key, held by a compute product published on the platform, used to call the products GraphQL API. Rotatable via the productRegenerateAPIKey mutation on the platform API.
  exchange_endpoint: POST https://api.strangeworks.com/product/token
  in: body
  name: ProductAPIKey
  parameter: key
  sources:
  - pypi:strangeworks-core==0.5.4
  type: apiKey
- applies_to:
  - https://api.strangeworks.com/sdk
  - https://api.strangeworks.com/platform
  - https://api.strangeworks.com/products
  - https://api.strangeworks.com/products/{product_slug}/resource/{resource_slug}/{path}
  bearerFormat: JWT
  description: 'The JWT returned by the token exchange, sent as `Authorization: Bearer <token>` on every GraphQL and REST-proxy call. The SDK caches it in an LRU cache with a TTL hash and re-exchanges on expiry.'
  name: BearerToken
  scheme: bearer
  sources:
  - pypi:strangeworks-core==0.5.4
  type: http
slug: strangeworks-authentication
source_filename: strangeworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://docs.strangeworks.com/strangeworks-python\ndocs: https://docs.strangeworks.com/strangeworks-python\nnote: >-\n  Strangeworks publishes no OpenAPI, so this profile was not derived by\n  derive-authentication.py. It is assembled from the documented SDK auth flow plus the\n  first-party strangeworks-core 0.5.4 client (strangeworks_core/platform/auth.py,\n  gql.py, defaults.py) and confirmed against live probes of api.strangeworks.com.\nsummary:\n  types: [apiKey, http]\n  api_key_in: [body]\n  bearer_format: JWT\n  oauth2_flows: []\n  oidc: false\n  mtls: false\nbase_url: https://api.strangeworks.com\nschemes:\n- name: WorkspaceAPIKey\n  type: apiKey\n  in: body\n  parameter: key\n  description: >-\n    A per-workspace API key issued from the Strangeworks Portal home page. A user who\n    belongs to multiple workspaces has a different key for each. Exchanged for a\n    short-lived JWT — it is not sent on API calls directly.\n\
  \  issued_at: https://portal.strangeworks.com/\n  exchange_endpoint: POST https://api.strangeworks.com/users/token\n  sdk_usage: |\n    import strangeworks as sw\n    sw.authenticate(api_key)\n  sources: [https://docs.strangeworks.com/strangeworks-python, 'pypi:strangeworks-core==0.5.4']\n- name: ProductAPIKey\n  type: apiKey\n  in: body\n  parameter: key\n  description: >-\n    A product API key, held by a compute product published on the platform, used to\n    call the products GraphQL API. Rotatable via the productRegenerateAPIKey mutation\n    on the platform API.\n  exchange_endpoint: POST https://api.strangeworks.com/product/token\n  sources: ['pypi:strangeworks-core==0.5.4']\n- name: BearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    The JWT returned by the token exchange, sent as `Authorization: Bearer <token>` on\n    every GraphQL and REST-proxy call. The SDK caches it in an LRU cache with a TTL\n    hash and re-exchanges on expiry.\n  applies_to:\n\
  \  - https://api.strangeworks.com/sdk\n  - https://api.strangeworks.com/platform\n  - https://api.strangeworks.com/products\n  - https://api.strangeworks.com/products/{product_slug}/resource/{resource_slug}/{path}\n  sources: ['pypi:strangeworks-core==0.5.4']\ntoken_exchange:\n- endpoint: POST https://api.strangeworks.com/users/token\n  audience: SDK / platform user\n  request: '{\"key\": \"<workspace api key>\"}'\n  returns: JWT bearer token\n  observed_error:\n    probe: POST with empty body, 2026-08-05\n    http_status: 400\n    body: '{\"description\":\"\",\"message\":\"key cannot be empty\"}'\n- endpoint: POST https://api.strangeworks.com/product/token\n  audience: platform product\n  request: '{\"key\": \"<product api key>\"}'\n  returns: JWT bearer token\n  observed_error:\n    probe: POST with empty body, 2026-08-05\n    http_status: 400\n    body: '{\"description\":\"\",\"message\":\"key cannot be empty\"}'\nkey_management:\n  rotate_user_key: 'platform GraphQL mutation: workspaceMemberRegenerateAPIKey'\n\
  \  delete_user_key: 'platform GraphQL mutation: workspaceMemberDeleteAPIKey'\n  rotate_product_key: 'platform GraphQL mutation: productRegenerateAPIKey'\n  scope: >-\n    Authorization is workspace-scoped and role-based (WorkspaceRole enum in the\n    platform schema), not OAuth-scope based. There is no OAuth 2.0 or OIDC surface.\nx-observation:\n  anonymous_introspection: true\n  detail: >-\n    GraphQL introspection (__schema) answers HTTP 200 anonymously on /sdk, /platform and\n    /products with no Authorization header — the full type system, including every\n    mutation on user accounts, billing and workspaces, is readable without credentials.\n    Data-bearing fields still require a bearer token; only the schema is public. This is\n    an observation about the deployed surface, not a documented Strangeworks feature.\n  probed: '2026-08-05'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strangeworks/refs/heads/main/authentication/strangeworks-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Quantum Computing
- Optimization
- High Performance Computing
- Artificial Intelligence
- Developer Platform
- GraphQL
- Compute
- Scientific Computing
- Operations Research
---
