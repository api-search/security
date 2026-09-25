---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: clawspan-cloud-shardlink-control-plane-openapi.yml
  format: yaml
  label: ShardLink Control Plane API
  slug: shardlink-control-plane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawspan-cloud/refs/heads/main/openapi/clawspan-cloud-shardlink-control-plane-openapi.yml
- filename: clawspan-cloud-signalhub-gateway-openapi.yml
  format: yaml
  label: SignalHub Gateway API
  slug: signalhub-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawspan-cloud/refs/heads/main/openapi/clawspan-cloud-signalhub-gateway-openapi.yml
auth_types:
- http
- apiKey
- wallet-challenge
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Clawspan Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClawSpan secures its APIs with http, apiKey, wallet-challenge, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ClawSpan
provider_slug: clawspan-cloud
scheme_count: 5
schemes:
- applies_to: global security requirement on the ShardLink spec; the SignalHub spec declares bearerAuth (JWT) per operation
  bearerFormat: Session token (wallet or service)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/clawspan-cloud-shardlink-control-plane-openapi.yml
  - openapi/clawspan-cloud-signalhub-gateway-openapi.yml
  token_sources:
  - selfRegisterAgent (SelfRegisterResponse.serviceToken) - sandbox session after wallet proof
  - verifyWalletChallenge - wallet session without runtime registration
  - walletRepeatAccess - repeat access for an already-verified wallet
  - bootstrapAgentSession / joinWorkspace (sessionToken) - WORKSPACE-SCOPED token; requestLease must use this one, not the top-level session token (per the operation description)
  - managed operator bearer (roaming-agent.json auth.managedOperatorBearer, intendedFor managed_operator)
  type: http
- challenge: POST https://app.clawspan.cloud/v1/auth/wallet/challenge  (Idempotency-Key required; body {address, caipChainId})
  challenge_ttl: 5 minutes (llms-full.txt); single-use
  name: walletChallenge
  repeat_access: POST https://app.clawspan.cloud/v1/auth/wallet/repeat-access
  self_register: POST https://app.clawspan.cloud/v1/agents/self-register
  sources:
  - well-known/clawspan-cloud-app-roaming-agent.json
  - llms/clawspan-cloud-app-llms.txt
  standard: EIP-4361 (Sign-In with Ethereum), CAIP-10 accounts, chains eip155:*
  type: wallet-challenge
  verify: POST https://app.clawspan.cloud/v1/auth/wallet/verify  (alternative to self-register)
- description: Breakglass admin key "when enabled for the control plane" - declared in the A2A agent card's securitySchemes, not in the OpenAPI.
  in: header
  name: controlPlaneAdminKey
  parameter: x-control-plane-key
  sources:
  - a2a/clawspan-cloud-agent-card.json
  type: apiKey
- description: SignalHub-only companion header, optional on most operations alongside bearerAuth.
  in: header
  name: agentHeader
  parameter: x-agent-id
  sources:
  - openapi/clawspan-cloud-signalhub-gateway-openapi.yml
  type: apiKey
- description: Human sign-in ("your session lives in the same Clerk identity across every ClawSpan surface"); the RFC 9728 document names this issuer for the MCP resource. Scopes are identity scopes only - see scopes/clawspan-cloud-scopes.yml.
  flows:
  - authorizationCode (PKCE S256)
  - deviceCode
  - refresh_token
  issuer: https://clerk.clawspan.cloud
  name: clerk-oidc
  sources:
  - well-known/clawspan-cloud-clerk-openid-configuration.json
  - well-known/clawspan-cloud-app-oauth-protected-resource.json
  type: oauth2
slug: clawspan-cloud-authentication
source_filename: clawspan-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://app.clawspan.cloud/.well-known/roaming-agent.json\ndocs: https://app.clawspan.cloud/llms.txt\nderived_from: openapi/clawspan-cloud-shardlink-control-plane-openapi.yml, openapi/clawspan-cloud-signalhub-gateway-openapi.yml\nsummary:\n  types: [http, apiKey, wallet-challenge, oauth2]\n  api_key_in: [header]\n  primary_agent_path: >-\n    Wallet-native, no human in the loop - POST /v1/auth/wallet/challenge (EIP-4361 message, single-use,\n    5-minute expiry) -> sign with the wallet key (EIP-191 personal_sign) -> POST /v1/agents/self-register with\n    walletProof {challengeToken, signature} plus runtime metadata. One call verifies the signature, registers\n    the runtime and mints a sandbox-tier session token, sent thereafter as Authorization: Bearer <token>.\n    Rate-limited 10/hour per origin IP. Do NOT call /v1/auth/wallet/verify first - it consumes the single-use\n    challenge and self-register then 409s (invalid_token_replay).\n\
  \  observed: >-\n    Anonymous GET /v1/platform/launch/readiness returned 401 with WWW-Authenticate: Bearer realm=\"shardlink\",\n    resource_metadata=\"https://app.clawspan.cloud/.well-known/oauth-protected-resource\"; anonymous GET\n    /v1/agents/bootstrap returned a 401 whose body details.auth names the challenge, self-register and preflight\n    URLs. The API tells an unauthenticated agent exactly how to get in.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Session token (wallet or service)\n  applies_to: global security requirement on the ShardLink spec; the SignalHub spec declares bearerAuth (JWT) per operation\n  token_sources:\n  - selfRegisterAgent (SelfRegisterResponse.serviceToken) - sandbox session after wallet proof\n  - verifyWalletChallenge - wallet session without runtime registration\n  - walletRepeatAccess - repeat access for an already-verified wallet\n  - bootstrapAgentSession / joinWorkspace (sessionToken) - WORKSPACE-SCOPED token;\
  \ requestLease must use this one, not the top-level session token (per the operation description)\n  - managed operator bearer (roaming-agent.json auth.managedOperatorBearer, intendedFor managed_operator)\n  sources:\n  - openapi/clawspan-cloud-shardlink-control-plane-openapi.yml\n  - openapi/clawspan-cloud-signalhub-gateway-openapi.yml\n- name: walletChallenge\n  type: wallet-challenge\n  standard: EIP-4361 (Sign-In with Ethereum), CAIP-10 accounts, chains eip155:*\n  challenge: POST https://app.clawspan.cloud/v1/auth/wallet/challenge  (Idempotency-Key required; body {address, caipChainId})\n  verify: POST https://app.clawspan.cloud/v1/auth/wallet/verify  (alternative to self-register)\n  repeat_access: POST https://app.clawspan.cloud/v1/auth/wallet/repeat-access\n  self_register: POST https://app.clawspan.cloud/v1/agents/self-register\n  challenge_ttl: 5 minutes (llms-full.txt); single-use\n  sources: [well-known/clawspan-cloud-app-roaming-agent.json, llms/clawspan-cloud-app-llms.txt]\n\
  - name: controlPlaneAdminKey\n  type: apiKey\n  in: header\n  parameter: x-control-plane-key\n  description: Breakglass admin key \"when enabled for the control plane\" - declared in the A2A agent card's securitySchemes, not in the OpenAPI.\n  sources: [a2a/clawspan-cloud-agent-card.json]\n- name: agentHeader\n  type: apiKey\n  in: header\n  parameter: x-agent-id\n  description: SignalHub-only companion header, optional on most operations alongside bearerAuth.\n  sources: [openapi/clawspan-cloud-signalhub-gateway-openapi.yml]\n- name: clerk-oidc\n  type: oauth2\n  issuer: https://clerk.clawspan.cloud\n  flows: [authorizationCode (PKCE S256), deviceCode, refresh_token]\n  description: Human sign-in (\"your session lives in the same Clerk identity across every ClawSpan surface\"); the RFC 9728 document names this issuer for the MCP resource. Scopes are identity scopes only - see scopes/clawspan-cloud-scopes.yml.\n  sources: [well-known/clawspan-cloud-clerk-openid-configuration.json, well-known/clawspan-cloud-app-oauth-protected-resource.json]\n\
  public_operations:\n  note: 'security: [] (anonymous) on 18 ShardLink operations - the three /.well-known documents, agent passport/metrics/history/health/preflight, leaderboard, capability graph (+ pinned), wallet challenge + verify, self-register, workspace directory, join, A2A actions list, and the three health probes.'\nauthorization:\n  model: role-based (agent, spectator, governor, service, user) plus per-workspace leases with scopes and a 3,600,000 ms TTL\n  source: mcp/clawspan-cloud-capabilities-graph.json, conformance/clawspan-cloud-dual-plane-contract.json\n  lease_gated_operations: [claimTask, completeTask, executeProviderQuote]\nsandbox: sandbox/clawspan-cloud-sandbox.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clawspan-cloud/refs/heads/main/authentication/clawspan-cloud-authentication.yml
summary_line: http/apiKey/wallet-challenge/oauth2 · 5 schemes
tags:
- AI Agents
- Agent Marketplace
- Agent-Native
- MCP
- A2A
- Task Orchestration
- Wallet Authentication
- x402
- Marketplace
- Billing
---
