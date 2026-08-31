---
api_key_in: []
api_specs:
- filename: proofdraw-account-api-openapi.yml
  format: yaml
  label: ProofDraw Account API
  slug: proofdraw-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proofdraw/refs/heads/main/openapi/proofdraw-account-api-openapi.yml
- filename: proofdraw-auth-api-openapi.yml
  format: yaml
  label: ProofDraw Auth API
  slug: proofdraw-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proofdraw/refs/heads/main/openapi/proofdraw-auth-api-openapi.yml
- filename: proofdraw-draws-api-openapi.yml
  format: yaml
  label: ProofDraw Draws API
  slug: proofdraw-draws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proofdraw/refs/heads/main/openapi/proofdraw-draws-api-openapi.yml
- filename: proofdraw-system-api-openapi.yml
  format: yaml
  label: ProofDraw System API
  slug: proofdraw-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proofdraw/refs/heads/main/openapi/proofdraw-system-api-openapi.yml
- filename: proofdraw-verification-api-openapi.yml
  format: yaml
  label: ProofDraw Verification API
  slug: proofdraw-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proofdraw/refs/heads/main/openapi/proofdraw-verification-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Proofdraw Authentication
name_suffix: Authentication
oauth_flows: []
overview: ProofDraw secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ProofDraw
provider_slug: proofdraw
scheme_count: 1
schemes:
- description: 'API key: `Authorization: Bearer pd_live_…` (or `pd_test_…` for sandbox keys).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/proofdraw-api-openapi.yml
  type: http
slug: proofdraw-authentication
source_filename: proofdraw-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: openapi/proofdraw-api-openapi.yml\ndocs: https://proofdraw.com/api\nsummary:\n  types:\n    - http\n  http_schemes:\n    - bearer\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    Single-mechanism auth: a static, long-lived API key presented as an HTTP bearer token. No OAuth 2.0,\n    no OIDC, no mTLS, so there is no scope surface to capture (scopes/ is correctly absent).\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: 'API key: `Authorization: Bearer pd_live_…` (or `pd_test_…` for sandbox keys).'\n    sources:\n      - openapi/proofdraw-api-openapi.yml\nkey_model:\n  prefixes:\n    - prefix: pd_live_\n      mode: live\n    - prefix: pd_test_\n      mode: sandbox\n  issuance:\n    - operation: POST /v1/auth/register\n      description: >-\n        Creates a TIER_FREE account and returns a freshly-issued pd_live_ key. Requires name, email,\n        password (8–255 chars) and a `terms_accepted_at`\
  \ ISO-8601 timestamp at or after the current Terms\n        effective date — server-side consent enforcement, not just a frontend checkbox.\n    - operation: POST /v1/auth/login\n      description: >-\n        Exchanges email + password for a NEW key on every call. Previously issued keys keep working;\n        there is no documented key-revocation or key-listing endpoint.\n  storage: >-\n    Keys are hashed with SHA-256 at rest; only the prefix (e.g. `pd_live_8K3Q`) is recoverable for\n    display. The raw key is returned exactly once, on the issuing response.\n  passwords: bcrypt at rest, never returned\n  rotation:\n    documented: false\n    note: >-\n      Login mints a new key without invalidating prior ones, so rotation is additive-only. No revoke,\n      list, or expire endpoint is published — an operator cannot retire a leaked key through the API.\nunauthenticated_surface:\n  - GET /health\n  - GET /list/{hash}\n  - GET /list/{hash}/ots\n  - GET /v/{publicId}   # human-facing verification\
  \ receipt; documented but absent from the OpenAPI\n  - POST /v1/auth/login\n  - POST /v1/auth/register\ngaps:\n  - No key revocation, expiry, or listing endpoint is documented.\n  - No scoped or least-privilege keys — one key carries the whole account surface.\n  - No OAuth 2.0 / OIDC, so no delegated third-party access model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proofdraw/refs/heads/main/authentication/proofdraw-authentication.yml
summary_line: http · 1 scheme
tags:
- randomness
- provably-fair
- drand
- Verifiable Randomness
- cryptography
- raffle
- giveaway
- sweepstakes
- lottery
- Verification
- Webhook
- REST API
---
