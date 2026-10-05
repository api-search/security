---
anonymous_access: false
api_key_in: []
api_specs:
- filename: assetfare-auth-api-openapi.yml
  format: yaml
  label: AssetFare Auth API
  slug: assetfare-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-auth-api-openapi.yml
- filename: assetfare-quote-api-openapi.yml
  format: yaml
  label: AssetFare Quote API
  slug: assetfare-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-quote-api-openapi.yml
- filename: assetfare-session-api-openapi.yml
  format: yaml
  label: AssetFare Session API
  slug: assetfare-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-session-api-openapi.yml
- filename: assetfare-status-api-openapi.yml
  format: yaml
  label: AssetFare Status API
  slug: assetfare-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-status-api-openapi.yml
- filename: assetfare-well-known-api-openapi.yml
  format: yaml
  label: AssetFare .well Known API
  slug: assetfare-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-well-known-api-openapi.yml
- filename: assetfare-app-store-api-openapi.yml
  format: yaml
  label: AssetFare App Store API
  slug: assetfare-app-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-app-store-api-openapi.yml
- filename: assetfare-capabilities-api-openapi.yml
  format: yaml
  label: AssetFare Capabilities API
  slug: assetfare-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-capabilities-api-openapi.yml
- filename: assetfare-events-api-openapi.yml
  format: yaml
  label: AssetFare Events API
  slug: assetfare-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-events-api-openapi.yml
- filename: assetfare-google-play-api-openapi.yml
  format: yaml
  label: AssetFare Google Play API
  slug: assetfare-google-play-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-google-play-api-openapi.yml
- filename: assetfare-jobs-api-openapi.yml
  format: yaml
  label: AssetFare Jobs API
  slug: assetfare-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-jobs-api-openapi.yml
- filename: assetfare-prepare-api-openapi.yml
  format: yaml
  label: AssetFare Prepare API
  slug: assetfare-prepare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-prepare-api-openapi.yml
- filename: assetfare-search-filter-v-2-api-openapi.yml
  format: yaml
  label: AssetFare Search Filter v.2 API
  slug: assetfare-search-filter-v-2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-search-filter-v-2-api-openapi.yml
- filename: assetfare-suggestions-api-openapi.yml
  format: yaml
  label: AssetFare Suggestions API
  slug: assetfare-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-suggestions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Assetfare Authentication
name_suffix: Authentication
oauth_flows: []
overview: AssetFare secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AssetFare
provider_slug: assetfare
scheme_count: 1
schemes:
- description: Revocable wallet-bound credential required for session endpoints.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/assetfare-agent-native-route-api-openapi.json
  type: http
slug: assetfare-authentication
source_filename: assetfare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: >-\n  openapi/assetfare-agent-native-route-api-openapi.json securitySchemes +\n  https://assetfare.dev/llms.txt (Self-service execution) fetched 2026-09-14\ndocs: https://assetfare.dev/llms.txt\nsummary:\n  types:\n    - http\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: Revocable wallet-bound credential required for session endpoints.\n    sources:\n      - openapi/assetfare-agent-native-route-api-openapi.json\nwallet_auth_flow:\n  style: solana-signmessage-challenge\n  steps:\n    - POST /v1/auth/challenge with a Solana source_wallet -> returns an exact challenge message that authorizes no transaction.\n    - Sign that message with the wallet's signMessage capability (off-chain; no transaction/approval/transfer).\n    - POST /v1/auth/verify with challenge_id, source_wallet, signature, and terms_version -> returns a Bearer token.\n    - Use the token for /v1/session and every session\
  \ subresource.\n  binding: The token is bound to the verified source wallet; a different source wallet is rejected.\n  constraints: At most 5 unverified live login challenges may exist for one wallet.\npublic_endpoints:\n  no_auth: [getQuote, getStatus, getSignedManifest, createWalletChallenge, verifyWalletSignature]\n  note: Quote, status, and signed manifest require no token; challenge/verify mint the token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/authentication/assetfare-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Agents
- Asset Transfer
- Bridge
- Cross-Chain
- Non-Custodial
- Cryptocurrency
- Solana
- Base
- OpenAPI
- MCP
- Agent Skills
---
