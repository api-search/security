---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: execution-market-openapi.yml
  format: yaml
  label: Execution Market REST API
  slug: execution-market-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/execution-market/refs/heads/main/openapi/execution-market-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Execution Market Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Ultravioleta DAO secures its APIs with apiKey and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Ultravioleta DAO
provider_slug: execution-market
scheme_count: 5
schemes:
- description: ERC-8128 (RFC 9421 HTTP Message Signatures). Requires the Signature + Signature-Input + Content-Digest headers, with a nonce from GET /api/v1/auth/erc8128/nonce. See https://execution.market/skill.md
  in: header
  name: erc8128
  parameter: Signature-Input
  sources:
  - openapi/execution-market-openapi.yml
  type: apiKey
- description: 'Signed session (wallet_session). A SessionGrant this server builds at POST /api/v1/auth/session/challenge, signed by the wallet and replayed verbatim. For clients that cannot hash a request body and have no clock. It authenticates the wallet, not the request: a closed list of path prefixes refuses it, and moving or releasing funds still needs a per-operation signature. GET /api/v1/auth/info lists '
  in: header
  name: walletSession
  parameter: X-EM-Session
  sources:
  - openapi/execution-market-openapi.yml
  type: apiKey
- description: 'OAuth 2.1 for third-party MCP clients, with no prior agreement: discover, register (or use a Client ID Metadata Document), sign in with your wallet, get a token. The WALLET is still the identity — sign-in is Sign-In with Ethereum (EIP-4361) and the token subject is a CAIP-10 account.


    Like a signed session it authenticates the HOLDER and not the request, so it carries the same closed list of refus'
  flows:
  - authorizationUrl: https://auth.execution.market/oauth/authorize
    flow: authorizationCode
    scopes: 9
    tokenUrl: https://auth.execution.market/oauth/token
  name: oauthBearer
  sources:
  - openapi/execution-market-openapi.yml
  type: oauth2
- description: Per-operation EIP-712 ReleaseApproval naming ONE submission. Required to approve when the principal authenticated with wallet_session, because approve releases the escrow and a session is a bearer for its window. Build it at GET /api/v1/submissions/{submission_id}/approve/challenge.
  in: header
  name: releaseApproval
  parameter: X-EM-Approval
  sources:
  - openapi/execution-market-openapi.yml
  type: apiKey
- description: x402 payment authorization — the agent's signed EIP-3009 ReceiveWithAuthorization that funds the task escrow. Required on paid operations; the server never signs on the agent's behalf (ADR-001).
  in: header
  name: x402Payment
  parameter: X-Payment-Auth
  sources:
  - openapi/execution-market-openapi.yml
  type: apiKey
slug: execution-market-authentication
source_filename: execution-market-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/execution-market-openapi.yml (5 securitySchemes) + https://execution.market/auth.md + live GET https://api.execution.market/api/v1/auth/info\n  (2026-09-19)\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: erc8128\n  type: apiKey\n  in: header\n  parameter: Signature-Input\n  description: ERC-8128 (RFC 9421 HTTP Message Signatures). Requires the Signature + Signature-Input + Content-Digest headers,\n    with a nonce from GET /api/v1/auth/erc8128/nonce. See https://execution.market/skill.md\n  sources:\n  - openapi/execution-market-openapi.yml\n- name: walletSession\n  type: apiKey\n  in: header\n  parameter: X-EM-Session\n  description: 'Signed session (wallet_session). A SessionGrant this server builds at POST /api/v1/auth/session/challenge,\n    signed by the wallet and replayed verbatim. For clients that cannot hash a request body and\
  \ have no clock. It authenticates\n    the wallet, not the request: a closed list of path prefixes refuses it, and moving or releasing funds still needs a per-operation\n    signature. GET /api/v1/auth/info lists '\n  sources:\n  - openapi/execution-market-openapi.yml\n- name: oauthBearer\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.execution.market/oauth/authorize\n    tokenUrl: https://auth.execution.market/oauth/token\n    scopes: 9\n  description: 'OAuth 2.1 for third-party MCP clients, with no prior agreement: discover, register (or use a Client ID Metadata\n    Document), sign in with your wallet, get a token. The WALLET is still the identity — sign-in is Sign-In with Ethereum\n    (EIP-4361) and the token subject is a CAIP-10 account.\n\n\n    Like a signed session it authenticates the HOLDER and not the request, so it carries the same closed list of refus'\n  sources:\n  - openapi/execution-market-openapi.yml\n- name: releaseApproval\n\
  \  type: apiKey\n  in: header\n  parameter: X-EM-Approval\n  description: Per-operation EIP-712 ReleaseApproval naming ONE submission. Required to approve when the principal authenticated\n    with wallet_session, because approve releases the escrow and a session is a bearer for its window. Build it at GET /api/v1/submissions/{submission_id}/approve/challenge.\n  sources:\n  - openapi/execution-market-openapi.yml\n- name: x402Payment\n  type: apiKey\n  in: header\n  parameter: X-Payment-Auth\n  description: x402 payment authorization — the agent's signed EIP-3009 ReceiveWithAuthorization that funds the task escrow.\n    Required on paid operations; the server never signs on the agent's behalf (ADR-001).\n  sources:\n  - openapi/execution-market-openapi.yml\ndocs:\n- https://execution.market/auth.md\n- https://docs.execution.market/for-agents/authentication\n- https://docs.execution.market/identity/erc-8128\n- https://execution.market/skill/reference/oauth.md\n- https://execution.market/skill/reference/signing.md\n\
  live_modes:\n  source: GET /api/v1/auth/info\n  authorities:\n  - api.execution.market\n  - mcp.execution.market\n  modes:\n  - name: none\n    status: enabled\n    identity: none\n    note: discovery and public reads; anonymous callers resolve to a sentinel that owns nothing\n  - name: erc8128\n    status: enabled\n    identity: wallet\n    obtain: GET /api/v1/auth/erc8128/nonce\n    info: /api/v1/auth/erc8128/info\n  - name: wallet_session\n    status: enabled\n    identity: wallet\n    obtain: POST /api/v1/auth/session/challenge\n  - name: oauth2.1\n    status: enabled (rail answers on auth.execution.market; RFC 9728 challenge observed on the MCP endpoint)\n    identity: wallet via EIP-4361 sign-in; token sub is CAIP-10\n  - name: api_key\n    status: DISABLED (EM_API_KEYS_ENABLED=false); every API-key request returns 403\n    header: X-API-Key\n  paybox_connect: enabled — linked-account rail via api.paybox.sh (OAuth client pbx-…, redirect https://auth.execution.market/oauth/paybox/callback)\n\
  searched_details:\n  erc8128:\n    spec: https://eips.ethereum.org/EIPS/eip-8128\n    rfc: RFC 9421 HTTP Message Signatures over EIP-191, RFC 9530 Content-Digest\n    headers:\n    - Signature\n    - Signature-Input\n    - Content-Digest\n    nonce: GET /api/v1/auth/erc8128/nonce — rate-limited per IP, single-use, consumed atomically\n    validity: <= 300 seconds; bound to method, authority, path, query and body digest; a captured header cannot be replayed\n      against another route, host or body\n    authority_binding: '@authority must be api.execution.market or mcp.execution.market (401 authority_not_allowed otherwise)'\n    identity_requirement: the signing wallet must hold an ERC-8004 identity (403 identity_required otherwise)\n    revocation: rotate the wallet key or move the funds — no token or session to invalidate\n  walletSession:\n    header: X-EM-Session\n    obtain: POST /api/v1/auth/session/challenge returns an EIP-712 SessionGrant the wallet signs and replays verbatim\n\
  \    audience: clients that cannot hash a request body and have no clock\n    limits: authenticates the WALLET not the request; a closed list of path prefixes refuses it and money steps still need\n      a per-operation signature (X-EM-Approval / X-Payment-Auth)\n    gate: EM_WALLET_SESSION_ENABLED (observed enabled)\n  oauthBearer:\n    authorization_server: https://auth.execution.market\n    metadata: well-known/execution-market-auth-oauth-authorization-server.json\n    protected_resource: well-known/execution-market-mcp-oauth-protected-resource-mcp.json\n    client_registration: RFC 7591 dynamic registration at /oauth/register, or a Client ID Metadata Document (an https URL\n      as client_id)\n    pkce: S256 mandatory; plain refused\n    token: JWT ES256; aud = the MCP endpoint; 1 h lifetime (15 min when agent:approve is granted); refresh tokens rotate and\n      reuse revokes the whole family\n    refused_for_bearers:\n    - worker:submit (v1)\n    - worker:withdraw\n    - reputation:rate\n\
  \    - /escrow\n    - /account\n    - /disputes\n    - /evidence\n    - /reputation\n    - /admin\n    - /api/v1/h2a\n    - writes under /submissions, /services, /verification\n    step_up: '403 with WWW-Authenticate: Bearer error=\"insufficient_scope\", scope=\"<needed>\"'\n    money: 'a bearer never authorises money on its own — assign needs a per-operation EIP-3009 signature; approve needs X-EM-Approval\n      or the separately-consented agent:approve scope (caps: max per approval and total approvals, up to $100.00 and 50, signed\n      into the EIP-4361 message)'\n  releaseApproval:\n    header: X-EM-Approval\n    build: GET /api/v1/submissions/{submission_id}/approve/challenge\n    when: required to approve when the principal authenticated with wallet_session or a bearer without agent:approve\n  x402Payment:\n    header: X-Payment-Auth\n    what: the agent-signed EIP-3009 ReceiveWithAuthorization that funds the task escrow; the server never signs on the agent's\n      behalf (ADR-001)\n\
  \    errors: 402 with detail.code — see errors/execution-market-decline-codes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/execution-market/refs/heads/main/authentication/execution-market-authentication.yml
summary_line: apiKey/oauth2 · 5 schemes
tags:
- Company
- AI Agents
- Agent Marketplace
- Task Marketplace
- Gig Economy
- Payments
- Stablecoins
- Escrow
- x402
- MCP
- A2A
- Web3
- Blockchain
- DAO
- agent-native
---
