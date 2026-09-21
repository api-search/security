---
anonymous_access: false
api_key_in:
- header
- header-bearer
- body
api_specs:
- filename: snhp-dev-openapi.yml
  format: yaml
  label: SNHP Game Theory Layer API
  slug: game-theory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snhp-dev/refs/heads/main/openapi/snhp-dev-openapi.yml
- filename: snhp-dev-arena-openapi.yml
  format: yaml
  label: SNHP Evolution Arena API
  slug: evolution-arena-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snhp-dev/refs/heads/main/openapi/snhp-dev-arena-openapi.yml
auth_types:
- apiKey
- http-bearer
- body-field
- none
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Snhp Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: SNHP secures its APIs with apiKey, http-bearer, body-field, and none across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SNHP
provider_slug: snhp-dev
scheme_count: 5
schemes:
- bearerFormat: gt_<opaque>
  header: 'Authorization: Bearer gt_*'
  name: BearerKey
  note: Preferred form. Raises the caller to the 600/min-per-key rate lane; required (or X-API-Key) for the paid store calls when not passing api_key in the body.
  scheme: bearer
  status: documented-not-declared
  type: http
- in: header
  name: XApiKey
  note: Equivalent to BearerKey. GET /v1/billing/balance with no key answers 422 {"detail":[{"type":"missing","loc":["header","X-API-Key"],"msg":"Field required"}]} — the header is a declared FastAPI dependency there, and the missing-credential response is a 422 validation error, not a 401, with no WWW-Authenticate.
  parameter: X-API-Key
  status: documented-not-declared
  type: apiKey
- in: body
  name: BodyApiKey
  note: Several paid operations (SessionOpenIn, SessionMoveIn, ParkIn, FetchIn, CheckoutIn, RotateIn, StoreRequestIn ...) carry an api_key field in the JSON body and the MCP tools take it as a tool argument. The provider is explicit that a body key does NOT raise the rate limit ("the limiter only reads headers") and that "header wins" when both are sent. POST /v1/advice/session with no key answers 422 missing body.api_key.
  parameter: api_key
  status: documented-not-declared
  type: apiKey
- header: 'Authorization: Payment <credential carrying a Stripe Shared Payment Token>'
  name: MPPPayment
  note: 'Not identity — a payment credential (Machine Payments Protocol). POST /v1/mpp/topup with no credential answers 402 application/problem+json with a signed `WWW-Authenticate: Payment id=..., realm="snhp.dev", method="stripe", intent="charge", request=<b64 challenge>, description=..., expires=...` header and `Accept-Payment: stripe`; the client authorises the challenge with an SPT scoped to the store and retries. Observed live 2026-09-19.'
  scheme: Payment
  status: documented-and-observed
  type: http
- name: PeerProof
  note: 'The verified-peer A2A flow authenticates OPERATORS, not callers: an Ed25519 keypair per operator, a signed attestation JWT from POST /v1/registry/register_operator (optionally upgraded to domain-level by a DNS-TXT challenge), and a short-lived per-negotiation proof signed locally. Verified server-side by open_session; not a request credential.'
  status: documented
  type: custom
slug: snhp-dev-authentication
source_filename: snhp-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  https://snhp.dev/llms.txt (\"Cost model\", \"Onboarding\", \"THE STORE — full reference / Auth &\n  wallet\"), https://snhp.dev/.well-known/agents.json (auth block), the operation descriptions of\n  issue_key_v1_keys_post, rotate_key_v1_keys_rotate_post and store_park_v1_store_park_post in\n  openapi/snhp-dev-openapi.yml, and live unauthenticated responses on 2026-09-19.\ndocs: https://snhp.dev/llms.txt\nchecked: '2026-09-19'\nderive_note: >-\n  0-working/derive-authentication.py produced no profile because the served OpenAPI declares NO\n  components.securitySchemes and no security[] on any of its 74 operations. The scheme below is\n  therefore assembled from the provider's prose and its live behaviour, not from the contract —\n  which is itself a finding: an OpenAPI consumer sees an API with no authentication at all, while\n  roughly a third of the operations require a key. overlays/ proposes the missing schemes.\n\
  summary:\n  types: [apiKey, http-bearer, body-field, none]\n  api_key_in: [header, header-bearer, body]\n  oauth2_flows: []\n  human_required_to_obtain_key: false\n  card_required_to_obtain_key: false\n  self_serve_issuance: 'POST /v1/keys — \"Programmatic API key issuance (no human approval)\", returns gt_* in <500ms, idempotent on agent_id within 24h, 10 requests/hour per IP.'\n  key_prefix: gt_\n  free_surface: 'All Tier 0 math operations (negotiate, bundle, auction.*, mechanism.*, rent/check, helper, notary verify, discovery) work with NO key at the 60/min-per-IP floor.'\nschemes:\n  - name: BearerKey\n    type: http\n    scheme: bearer\n    bearerFormat: 'gt_<opaque>'\n    header: 'Authorization: Bearer gt_*'\n    status: documented-not-declared\n    note: Preferred form. Raises the caller to the 600/min-per-key rate lane; required (or X-API-Key) for the paid store calls when not passing api_key in the body.\n  - name: XApiKey\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n\
  \    status: documented-not-declared\n    note: >-\n      Equivalent to BearerKey. GET /v1/billing/balance with no key answers 422\n      {\"detail\":[{\"type\":\"missing\",\"loc\":[\"header\",\"X-API-Key\"],\"msg\":\"Field required\"}]} — the\n      header is a declared FastAPI dependency there, and the missing-credential response is a 422\n      validation error, not a 401, with no WWW-Authenticate.\n  - name: BodyApiKey\n    type: apiKey\n    in: body\n    parameter: api_key\n    status: documented-not-declared\n    note: >-\n      Several paid operations (SessionOpenIn, SessionMoveIn, ParkIn, FetchIn, CheckoutIn, RotateIn,\n      StoreRequestIn ...) carry an api_key field in the JSON body and the MCP tools take it as a\n      tool argument. The provider is explicit that a body key does NOT raise the rate limit\n      (\"the limiter only reads headers\") and that \"header wins\" when both are sent. POST\n      /v1/advice/session with no key answers 422 missing body.api_key.\n  - name:\
  \ MPPPayment\n    type: http\n    scheme: Payment\n    header: 'Authorization: Payment <credential carrying a Stripe Shared Payment Token>'\n    status: documented-and-observed\n    note: >-\n      Not identity — a payment credential (Machine Payments Protocol). POST /v1/mpp/topup with no\n      credential answers 402 application/problem+json with a signed `WWW-Authenticate: Payment\n      id=..., realm=\"snhp.dev\", method=\"stripe\", intent=\"charge\", request=<b64 challenge>,\n      description=..., expires=...` header and `Accept-Payment: stripe`; the client authorises the\n      challenge with an SPT scoped to the store and retries. Observed live 2026-09-19.\n  - name: PeerProof\n    type: custom\n    status: documented\n    note: >-\n      The verified-peer A2A flow authenticates OPERATORS, not callers: an Ed25519 keypair per\n      operator, a signed attestation JWT from POST /v1/registry/register_operator (optionally\n      upgraded to domain-level by a DNS-TXT challenge), and\
  \ a short-lived per-negotiation proof\n      signed locally. Verified server-side by open_session; not a request credential.\nkey_lifecycle:\n  issue: 'POST /v1/keys {agent_id, contact_email, intended_use_summary, telemetry_consent?} -> {api_key: gt_*, rate_limit_per_minute: 600, telemetry_consent, wallet (50c starter credit)}'\n  shown_once: true\n  rotate: 'POST /v1/keys/rotate — replacement issued, full balance carries over, old key invalidated IMMEDIATELY with no grace period.'\n  revoke: 'No standalone revoke; rotation is the revocation path.'\n  recover: 'Manual, human-verified: email the registered contact address from that same address.'\n  telemetry_consent: 'Set ONCE at issuance and immutable; revoke by DELETE /v1/telemetry/delete + stop passing share_outcome.'\nobserved:\n  - {request: 'POST /v1/negotiate/turn (no key, documented quickstart body)', status: 200, note: free floor works}\n  - {request: 'GET /v1/billing/balance (no key)', status: 422, body: 'missing header X-API-Key'}\n\
  \  - {request: 'POST /v1/advice/session (no key)', status: 422, body: 'missing body api_key'}\n  - {request: 'POST /v1/mpp/topup (no credential)', status: 402, headers: ['WWW-Authenticate: Payment ...', 'Accept-Payment: stripe']}\nsee:\n  scopes: 'none — no OAuth2 (derive-oauth-scopes.py: 0 schemes)'\n  rate_limits: rate-limits/snhp-dev-rate-limits.yml\n  conventions: conventions/snhp-dev-conventions.yml\n  overlay: overlays/snhp-dev-openapi-overlay.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snhp-dev/refs/heads/main/authentication/snhp-dev-authentication.yml
summary_line: apiKey/http-bearer/body-field/none · 5 schemes
tags:
- Negotiation
- Game Theory
- AI Agents
- MCP
- A2A
- Agent Payments
- Auctions
- Mechanism Design
- Pricing Optimization
- Artificial Intelligence
- agent-native
- Developer Tools
---
