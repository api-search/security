---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: QRCodeCrafter API
  slug: qrcodecrafter-api
  spec_type: OpenAPI
  url: https://qrcodecrafter.com/.well-known/openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Qr Code Crafter Authentication
name_suffix: Authentication
oauth_flows: []
overview: QR Code Crafter secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: QR Code Crafter
provider_slug: qr-code-crafter
scheme_count: 3
schemes:
- applies_to:
  - downloadQr
  - generateQr
  - generateVerifiedQr
  - generateBulkQr
  - sendFeedback
  description: Optional issued key for scoped or rate-limited access. Requests without it continue to work unless an administrator enables key enforcement for the deployment, in which case unauthenticated calls return 401 with a WWW-Authenticate challenge.
  effect: Raises the cost budget from 180 to 600 units per 60-second window when enforcement is enabled.
  in: header
  name: AgentApiKey
  obtained_by: Contact support@qrcodecrafter.com — keys are issued, not self-served and not sold.
  parameter: X-Agent-Api-Key
  required: conditional
  sources:
  - openapi/qr-code-crafter-openapi-original.json
  type: apiKey
- applies_to:
  - getDynamicQr
  - updateDynamicQr
  - deleteDynamicQr
  bearerFormat: capability-token
  description: Private 43-character management capability for ONE dynamic QR record, returned at creation or at explicit token rotation and never retrievable afterwards.
  name: DynamicQrBearer
  required: true
  scheme: bearer
  sources:
  - openapi/qr-code-crafter-openapi-original.json
  token_pattern: ^[A-Za-z0-9_-]{43}$
  type: http
- applies_to:
  - getDynamicQrVault
  - updateDynamicQrVault
  - deleteDynamicQrVault
  - createDynamicQrVaultChild
  - updateDynamicQrVaultChild
  - getDynamicQrVaultChildAnalytics
  - deleteDynamicQrVaultChild
  bearerFormat: capability-token
  description: Private 43-character vault capability returned only when the vault is created. It authorizes the vault AND all nested records; child credentials are never issued or exposed.
  name: DynamicQrVaultBearer
  required: true
  scheme: bearer
  sources:
  - openapi/qr-code-crafter-openapi-original.json
  token_pattern: ^[A-Za-z0-9_-]{43}$
  type: http
slug: qr-code-crafter-authentication
source_filename: qr-code-crafter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: openapi/qr-code-crafter-openapi-original.json\ndocs: https://qrcodecrafter.com/ai.txt\nnote: >-\n  Upgraded from the mechanical derive, which collapsed the two distinct bearer capability schemes into\n  one. There are three securitySchemes in the contract, and the difference between the two bearer\n  schemes matters: a record capability authorizes one redirect, a vault capability authorizes a\n  container and every child inside it. Also note the whole model has no accounts, no login, no user\n  identity and no OAuth — authorization is a bearer secret you hold, nothing more.\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: []\n  accounts_required: false\n  default_posture: open\n  note: >-\n    The OpenAPI declares no top-level `security` requirement, so the generation surface is open by\n    default and the management surface applies its scheme per operation.\nschemes:\n  - name: AgentApiKey\n   \
  \ type: apiKey\n    in: header\n    parameter: X-Agent-Api-Key\n    required: conditional\n    description: >-\n      Optional issued key for scoped or rate-limited access. Requests without it continue to work\n      unless an administrator enables key enforcement for the deployment, in which case unauthenticated\n      calls return 401 with a WWW-Authenticate challenge.\n    effect: >-\n      Raises the cost budget from 180 to 600 units per 60-second window when enforcement is enabled.\n    obtained_by: Contact support@qrcodecrafter.com — keys are issued, not self-served and not sold.\n    applies_to: [downloadQr, generateQr, generateVerifiedQr, generateBulkQr, sendFeedback]\n    sources: [openapi/qr-code-crafter-openapi-original.json]\n  - name: DynamicQrBearer\n    type: http\n    scheme: bearer\n    bearerFormat: capability-token\n    token_pattern: '^[A-Za-z0-9_-]{43}$'\n    required: true\n    description: >-\n      Private 43-character management capability for ONE dynamic QR record,\
  \ returned at creation or at\n      explicit token rotation and never retrievable afterwards.\n    applies_to: [getDynamicQr, updateDynamicQr, deleteDynamicQr]\n    sources: [openapi/qr-code-crafter-openapi-original.json]\n  - name: DynamicQrVaultBearer\n    type: http\n    scheme: bearer\n    bearerFormat: capability-token\n    token_pattern: '^[A-Za-z0-9_-]{43}$'\n    required: true\n    description: >-\n      Private 43-character vault capability returned only when the vault is created. It authorizes the\n      vault AND all nested records; child credentials are never issued or exposed.\n    applies_to:\n      - getDynamicQrVault\n      - updateDynamicQrVault\n      - deleteDynamicQrVault\n      - createDynamicQrVaultChild\n      - updateDynamicQrVaultChild\n      - getDynamicQrVaultChildAnalytics\n      - deleteDynamicQrVaultChild\n    sources: [openapi/qr-code-crafter-openapi-original.json]\nunauthenticated_operations:\n  - createDynamicQr\n  - createDynamicQrVault\n  - redirectDynamicQr\n\
  \  - headDynamicQr\nunauthenticated_operations_note: >-\n  Creation is deliberately anonymous — that is how a capability model bootstraps with no accounts.\n  The write is additionally protected against cross-origin abuse with a 403, and by rate limits.\ncapability_model:\n  rotation: >-\n    PATCH with rotateToken:true returns a new managementToken and managementUrl once and immediately\n    invalidates the previous token.\n  recovery: none\n  recovery_note: >-\n    There is no password reset, no email recovery and no support path back to a lost capability. Losing\n    the token means the record keeps redirecting and can never be edited, paused or deleted. This is\n    the sharpest operational edge in the whole contract and every client should be built around it.\n  identifiers_are_not_credentials: >-\n    The 22-character slug and vaultId are public — the slug appears in the printed /r/{slug} URL. The\n    spec says outright that a vaultId is \"not sufficient for authorization\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qr-code-crafter/refs/heads/main/authentication/qr-code-crafter-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- QR Code
- QR Code Generation
- Static Qr
- Dynamic QR
- dynamic redirects
- image export
- bulk generation
- Developer Tools
- OpenAPI
- WebMCP
- browser agents
- payments (QR)
- Agent Readiness
- llms-txt
- capability tokens
---
