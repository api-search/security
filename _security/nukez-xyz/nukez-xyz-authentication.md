---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nukez-xyz-attest-api-openapi.yml
  format: yaml
  label: Nukez Attest API
  slug: nukez-xyz-attest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-attest-api-openapi.yml
- filename: nukez-xyz-attest-code-api-openapi.yml
  format: yaml
  label: Nukez Attest Code API
  slug: nukez-xyz-attest-code-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-attest-code-api-openapi.yml
- filename: nukez-xyz-files-api-openapi.yml
  format: yaml
  label: Nukez Files API
  slug: nukez-xyz-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-files-api-openapi.yml
- filename: nukez-xyz-health-api-openapi.yml
  format: yaml
  label: Nukez Health API
  slug: nukez-xyz-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-health-api-openapi.yml
- filename: nukez-xyz-jobs-api-openapi.yml
  format: yaml
  label: Nukez Jobs API
  slug: nukez-xyz-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-jobs-api-openapi.yml
- filename: nukez-xyz-keys-api-openapi.yml
  format: yaml
  label: Nukez Keys API
  slug: nukez-xyz-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-keys-api-openapi.yml
- filename: nukez-xyz-lockers-v1-api-openapi.yml
  format: yaml
  label: Nukez Lockers V1 API
  slug: nukez-xyz-lockers-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-lockers-v1-api-openapi.yml
- filename: nukez-xyz-nukez-api-openapi.yml
  format: yaml
  label: Nukez Nukez API
  slug: nukez-xyz-nukez-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-nukez-api-openapi.yml
- filename: nukez-xyz-operators-api-openapi.yml
  format: yaml
  label: Nukez Operators API
  slug: nukez-xyz-operators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-operators-api-openapi.yml
- filename: nukez-xyz-owner-viewer-api-openapi.yml
  format: yaml
  label: Nukez Owner Viewer API
  slug: nukez-xyz-owner-viewer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-owner-viewer-api-openapi.yml
- filename: nukez-xyz-price-api-openapi.yml
  format: yaml
  label: Nukez Price API
  slug: nukez-xyz-price-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-price-api-openapi.yml
- filename: nukez-xyz-public-file-api-openapi.yml
  format: yaml
  label: Nukez Public File API
  slug: nukez-xyz-public-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-public-file-api-openapi.yml
- filename: nukez-xyz-receipts-api-openapi.yml
  format: yaml
  label: Nukez Receipts API
  slug: nukez-xyz-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-receipts-api-openapi.yml
- filename: nukez-xyz-retrieve-api-openapi.yml
  format: yaml
  label: Nukez Retrieve API
  slug: nukez-xyz-retrieve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-retrieve-api-openapi.yml
- filename: nukez-xyz-sandbox-ingest-api-openapi.yml
  format: yaml
  label: Nukez Sandbox Ingest API
  slug: nukez-xyz-sandbox-ingest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-sandbox-ingest-api-openapi.yml
- filename: nukez-xyz-short-url-api-openapi.yml
  format: yaml
  label: Nukez Short URL API
  slug: nukez-xyz-short-url-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-short-url-api-openapi.yml
- filename: nukez-xyz-sponsored-api-openapi.yml
  format: yaml
  label: Nukez Sponsored API
  slug: nukez-xyz-sponsored-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-sponsored-api-openapi.yml
- filename: nukez-xyz-storage-api-openapi.yml
  format: yaml
  label: Nukez Storage API
  slug: nukez-xyz-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-storage-api-openapi.yml
- filename: nukez-xyz-viewer-auth-api-openapi.yml
  format: yaml
  label: Nukez Viewer Auth API
  slug: nukez-xyz-viewer-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nukez-xyz/openapi/nukez-xyz-viewer-auth-api-openapi.yml
auth_types: []
description: Authentication methods for Nukez API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Nukez Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nukez declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Nukez
provider_slug: nukez-xyz
scheme_count: 2
schemes:
- evidence: The X‑Nukez headers carry the public identity, freshness values, and signature.
  header: X-Nukez-Identity, X-Nukez-Nonce, X-Nukez-Timestamp, X-Nukez-Signature
  how_to_obtain: Client builds a canonical request message, signs it with its private key, and includes the public identity and signature in the X‑Nukez‑Identity and X‑Nukez‑Signature headers along with nonce and timestamp.
  location: header
  name: Nukez request signature
  type: apiKey
- evidence: session token it produces is stored in localStorage under nukez_session_token and sent as a Bearer header on every session‑gated portal read.
  header: 'Authorization: Bearer <token>'
  how_to_obtain: User authenticates via WebAuthn passkey, which creates a session token stored in localStorage and used as a Bearer token.
  location: header
  name: Portal session token
  type: http-bearer
slug: nukez-xyz-authentication
source_filename: nukez-xyz-authentication.yml
source_heading: Authentication Profile
source_url: https://nukez.xyz/docs/nukezagent/signing-bridge
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nukez.xyz/docs/nukezagent/signing-bridge\nsources:\n- https://nukez.xyz/docs/nukezagent/signing-bridge\n- https://nukez.xyz/docs/http/helpers\n- https://nukez.xyz/docs/pynukez/helpers\n- https://nukez.xyz/docs/portal/multi-keypair\ndescription: Authentication methods for Nukez API\nschemes:\n- type: apiKey\n  name: Nukez request signature\n  evidence: The X‑Nukez headers carry the public identity, freshness values, and signature.\n  location: header\n  header: X-Nukez-Identity, X-Nukez-Nonce, X-Nukez-Timestamp, X-Nukez-Signature\n  how_to_obtain: Client builds a canonical request message, signs it with its private key, and includes the public identity and signature in the\n    X‑Nukez‑Identity and X‑Nukez‑Signature headers along with nonce and timestamp.\n- type: http-bearer\n  name: Portal session token\n  evidence: session token it produces is stored in localStorage under\
  \ nukez_session_token and sent as a Bearer header on every session‑gated portal\n    read.\n  location: header\n  header: 'Authorization: Bearer <token>'\n  how_to_obtain: User authenticates via WebAuthn passkey, which creates a session token stored in localStorage and used as a Bearer token.\ndocs: https://nukez.xyz/docs/nukezagent/signing-bridge\n"
source_yaml_url: https://artifacts.apis.io/nukez-xyz/authentication/nukez-xyz-authentication.yml
summary_line: 2 schemes
tags:
- AI Agents
- Infrastructure
- Autonomous
- Artificial Intelligence
- Storage
---
