---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: mandateshield-com-openapi.yml
  format: yaml
  label: MandateShield Payment Authority API
  slug: payment-authority-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mandateshield-com/refs/heads/main/openapi/mandateshield-com-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mandateshield Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: MandateShield secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MandateShield
provider_slug: mandateshield-com
scheme_count: 2
schemes:
- description: Hosting-injected authenticated account-owner identity. The hosting boundary validates the user session and injects this assertion; callers cannot authenticate by supplying this header directly. State-changing control-plane requests additionally require the trusted same-origin check documented by the operation.
  in: header
  name: hostingSession
  parameter: OAI-Authenticated-User-Email
  sources:
  - openapi/mandateshield-com-openapi.yml
  type: apiKey
- bearerFormat: ms_test_… or ms_live_…
  description: Keep API keys server-side and isolate them by purpose. VERIFY keys can issue challenges and strict decisions. Paid live PROCESSOR keys are bound to one processor_audience and can call only the execution-transition boundary.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mandateshield-com-openapi.yml
  type: http
slug: mandateshield-com-authentication
source_filename: mandateshield-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://mandateshield.com/docs\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  oauth: false\n  openid_connect: false\n  mutual_tls: false\n  model: Bearer API keys in two purpose-isolated roles (VERIFY and PROCESSOR), test/live split by key prefix, plus\n    a hosting-injected session assertion for the account control plane. No OAuth, no OIDC provider role, no scopes\n    surface.\nschemes:\n- name: hostingSession\n  type: apiKey\n  in: header\n  parameter: OAI-Authenticated-User-Email\n  description: Hosting-injected authenticated account-owner identity. The hosting boundary validates the user session\n    and injects this assertion; callers cannot authenticate by supplying this header directly. State-changing control-plane\n    requests additionally require the trusted same-origin check documented by the operation.\n  sources:\n  - openapi/mandateshield-com-openapi.yml\n- name:\
  \ bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: ms_test_… or ms_live_…\n  description: Keep API keys server-side and isolate them by purpose. VERIFY keys can issue challenges and strict\n    decisions. Paid live PROCESSOR keys are bound to one processor_audience and can call only the execution-transition\n    boundary.\n  sources:\n  - openapi/mandateshield-com-openapi.yml\ndocs:\n- https://mandateshield.com/docs\n- https://mandateshield.com/developers\n- https://mandateshield.com/security\nderived_from: openapi/mandateshield-com-openapi.yml\nkey_roles:\n- role: VERIFY\n  can:\n  - createVerificationChallenge\n  - verifyCryptographicAuthority\n  - verifyCryptographicAuthorityBatch\n  - verify_cryptographic_payment_authority (MCP)\n  - A2A strict skill\n  cannot:\n  - transition an execution authorization\n  - redeem a permit\n  placement: trusted server-side verification worker; may be passed to an MCP/A2A client only as a server-side Authorization\n    header\n- role: PROCESSOR\n\
  \  can:\n  - transitionExecutionAuthorization (CONSUME / COMMIT / RELEASE / EXPIRE)\n  - redeemExecutionPermit\n  - reportProviderSubmission\n  cannot:\n  - issue a challenge\n  - create an authorization\n  binding: bound at creation to one exact processor_audience; the signed receipt and expected_audience must match\n    it\n  placement: inside the trusted gateway; the redemption credential only inside the customer-deployed exclusive executor\n    with the provider credential — never the agent, model, browser, merchant page or verification worker\nkey_prefixes:\n  test: ms_test_\n  live: ms_live_\n  note: From bearerFormat in the spec and the A2A card. Test keys persist up to 5,000 decisions per month and never\n    produce enforcement_authorized=true.\nheader: 'Authorization: Bearer ms_live_...'\nanonymous_operations:\n- evaluatePurchase\n- evaluatePurchaseBatch\n- normalizeAgentPaymentProtocol\n- runStrictLifecycleSandbox\n- verifyDecisionReceipt\n- verifyExecutionPermit\n- verifyExecutionReceipt\n\
  - getReceiptTransparency\n- listPublicProofAttestations\n- getPublicProofAttestation\n- getPublicProofBadge\n- createPublicProofChallenge\n- issuePublicProofAttestation\n- listDeploymentActivationProofs\n- getDeploymentActivationProof\n- getDeploymentActivationProofBadge\n- getThreatIntelligence\noptional_auth_operations:\n  note: security lists both bearerAuth and {} — anonymous calls use the rate-limited non-persisted sandbox and can\n    never reserve authority\n  operations:\n  - evaluatePurchase\n  - evaluatePurchaseBatch\n  - verifyCryptographicAuthority\n  - verifyCryptographicAuthorityBatch\ncontrol_plane:\n  scheme: hostingSession\n  operations:\n  - getGlobalExecutionInterlock\n  - setGlobalExecutionInterlock\n  note: The OAI-Authenticated-User-Email header is injected by the hosting boundary after a \"Sign in with ChatGPT\"\n    session (dashboard redirects to auth.openai.com); callers cannot supply it. State changes also require a trusted\n    same-origin check.\nprovider_webhook:\n\
  \  operation: receiveStripeProviderWebhook\n  auth: Stripe-Signature header verified against the connection's signing secret; the event is treated as a hint,\n    never terminal proof\nkey_management:\n  where: https://mandateshield.com/dashboard\n  trust_anchors: Authority-issuer public JWKs are pinned per account with issuer, audience, protocol and RFC 7638\n    thumbprint; a JWK supplied in a request verifies signature math but establishes no trust. Private keys are rejected.\n    Mandates and keys can be revoked independently.\n  replay_boundary: account-wide idempotency tombstones survive API-key rotation\nagent_surfaces:\n  mcp: 'https://mandateshield.com/api/mcp — anonymous initialize/tools/list; optional Bearer VERIFY key for the\n    strict tool (server.json: Authorization isRequired false)'\n  a2a: securitySchemes.bearerAuth httpAuthSecurityScheme Bearer, ms_test_... or ms_live_...\n  oauth_discovery: /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource\
  \ both 404 (well-known/)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mandateshield-com/refs/heads/main/authentication/mandateshield-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Payments
- Agentic Commerce
- AI Agents
- Payment Authorization
- Fraud Prevention
- Cryptographic Verification
- MCP
- A2A
- x402
- AP2
- Stripe
- Agent-Native
- Switzerland
---
