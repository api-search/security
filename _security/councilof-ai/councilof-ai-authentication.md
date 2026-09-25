---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: councilof-ai-public-api-openapi.yml
  format: yaml
  label: Council of AI Public API
  slug: council-of-ai-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/councilof-ai/refs/heads/main/openapi/councilof-ai-public-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Councilof Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Council of AI secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Council of AI
provider_slug: councilof-ai
scheme_count: 3
schemes:
- description: Ed25519 signature of canonical body, under did:web:csoai.org#card-attestation-1
  in: header
  name: ed25519
  parameter: X-CSOAI-Signed-Card
  sources:
  - openapi/councilof-ai-public-api-openapi.yml
  type: apiKey
  used_by: declared in components.securitySchemes; no operation references it in a security requirement
- bearerFormat: JWT
  description: GitHub Actions OIDC token satisfying the handler's issuer, audience, repository and workflow checks.
  name: githubOidc
  note: Machine identity for the provider's own CI (board signing) — not obtainable by a third party.
  scheme: bearer
  sources:
  - openapi/councilof-ai-public-api-openapi.yml
  type: http
  used_by:
  - post__api_board-sign
- description: Operation-specific configured operator or writer credential. Not interchangeable across operations.
  name: operatorBearer
  note: Provider-internal; no issuance path is documented.
  scheme: bearer
  sources:
  - openapi/councilof-ai-public-api-openapi.yml
  type: http
  used_by:
  - get__api_action-jobs
  - patch__api_action-jobs
  - post__api_action-jobs
  - post__api_provider-canary
slug: councilof-ai-authentication
source_filename: councilof-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/councilof-ai-public-api-openapi.yml\ndocs: https://councilof.ai/api-docs/\nsummary:\n  default: anonymous\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  payment_gate: x402 (HTTP 402) on 10 REST doors and 4 MCP tools — an economic gate, not an authentication scheme\n  note: >-\n    The public surface needs no credential of any kind. api-docs: \"Public · keyless · CORS-open … No account, no\n    API key, no tiers … Auth: none.\" 92 of 141 operations declare security [] and a further 44 declare no\n    security block; every read of the board, the signed cards, the root and the proofs is anonymous, as are MCP\n    initialize/tools/list and the A2A JSON-RPC endpoint. The three declared securitySchemes guard\n    provider-internal action-job and canary doors only (5 operations): there is no public sign-up that yields one of them. Paid\n    artefacts are unlocked by an x402 payment (X-PAYMENT header on REST,\
  \ x_payment argument on MCP), settled by\n    the caller's own wallet in USDC on Base; the provider \"holds no key for you and never settles on your\n    behalf\" (quickstart.json step 4).\nschemes:\n- name: ed25519\n  type: apiKey\n  in: header\n  parameter: X-CSOAI-Signed-Card\n  description: Ed25519 signature of canonical body, under did:web:csoai.org#card-attestation-1\n  used_by: declared in components.securitySchemes; no operation references it in a security requirement\n  sources:\n  - openapi/councilof-ai-public-api-openapi.yml\n- name: githubOidc\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: GitHub Actions OIDC token satisfying the handler's issuer, audience, repository and workflow checks.\n  used_by: [post__api_board-sign]\n  note: Machine identity for the provider's own CI (board signing) — not obtainable by a third party.\n  sources:\n  - openapi/councilof-ai-public-api-openapi.yml\n- name: operatorBearer\n  type: http\n  scheme: bearer\n  description:\
  \ Operation-specific configured operator or writer credential. Not interchangeable across operations.\n  used_by: [get__api_action-jobs, patch__api_action-jobs, post__api_action-jobs, post__api_provider-canary]\n  note: Provider-internal; no issuance path is documented.\n  sources:\n  - openapi/councilof-ai-public-api-openapi.yml\npayment:\n  protocol: x402 v2\n  rest_header: X-PAYMENT (challenge in the 402 body and the PAYMENT-REQUIRED response header)\n  mcp_argument: x_payment\n  network: eip155:8453 (Base)\n  asset: USDC 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913\n  payTo: '0x212686404A7D1E1fD88F35eD6200c3aF7A78ae31'\n  discovery: https://councilof.ai/.well-known/x402.json\n  catalog: https://councilof.ai/api/x402\n  observed: GET /api/free-door → 402 (amount \"0\"); GET /api/request-attestation?subject=… → 402 (amount \"10000\" atomic = 0.01 USDC, campaign-priced). No purchase made.\nsigning_keys:\n  did_document: https://csoai.org/.well-known/did.json\n  keys: [did:web:csoai.org#site-release-1,\
  \ did:web:csoai.org#estate-chain-1, did:web:csoai.org#board-attestation-1, did:web:csoai.org#card-attestation-1]\n  note: These are the PROVIDER's signing keys (verify responses, offers, receipts and cards against them); they are not client credentials.\noauth: none\noidc: none\nmcp_auth: none (server card authentication.required false; no RFC 8414/9728 metadata)\na2a_auth: none (card declares no securitySchemes)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/councilof-ai/refs/heads/main/authentication/councilof-ai-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- AI Governance
- AI Measurement
- AI Safety
- EU AI Act
- Compliance
- Provenance
- Agents
- A2A
- MCP
- x402
- Agentic Commerce
- Agent-Native
- United Kingdom
---
