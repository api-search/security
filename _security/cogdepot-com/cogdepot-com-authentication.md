---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cogdepot-com-openapi.yml
  format: yaml
  label: cogDepot API
  slug: cogdepot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cogdepot-com/refs/heads/main/openapi/cogdepot-com-openapi.yml
auth_types:
- apiKey
- http
- x402
- oauth2-via-mcp
description: 'Three ways to be authorised on the same API: a platform API key in x-api-key (the normal case), the web console''s Cognito session as a Bearer JWT on the self-service account and dashboard routes only, and - on the twelve payable routes - a signed x402 USDC payment in place of any credential. A fourth path reaches the API indirectly: the hosted MCP server at mcp.cogdepot.com authorises the operator with OAuth 2.1 + PKCE and relays a per-action-scoped token. Discovery documents, POST /a2a, the public reputation lookup and the storefront preview need nothing.'
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Cogdepot Com Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode (PKCE S256) on the MCP host only
overview: cogDepot secures its APIs with apiKey, http, x402, and oauth2-via-mcp across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode (PKCE S256) on the MCP host only flow(s).
provider_name: cogDepot
provider_slug: cogdepot-com
scheme_count: 4
schemes:
- applied: 'global default (security: [{apiKey: []}]); overridden to [] on the discovery, a2a, meta, registration and reputation-lookup operations'
  description: 'Platform API key. Three origins: returned by open registration (POST /v1/account/register, free and credential-less), issued once at web sign-up and inherited by agents out-of-band, or - where this deployment enables x402 - minted by a first settled payment and returned once in that response body. Never re-issued by any of them; a lost key is rotated, not recovered. Disabled keys return 403. Only a salted hash of the key is stored, so it can never be shown again.'
  failure_codes:
    401 unauthorized: a key was presented and rejected
    '402': on a payable route, NO credential at all answers 402 with an x402 offer menu rather than 401
    403 api_key_disabled: operator disabled the key; rotateKey reactivates
    403 forbidden: valid key, action not permitted (e.g. a negotiator calling finalize)
  in: header
  issuance:
  - body: '{"accepted_terms": true}'
    door: open registration
    grants_credit: false
    operation: registerAccount (POST /v1/account/register, unauthenticated, free, rate limited per source)
  - door: web sign-up
    grants_credit: 20,000 credits ($10.00)
    note: key shown once at sign-up; handed to agents out of band
    options:
    - Google
    - GitHub
    - email
    url: https://cogdepot.com/auth/signup
  - door: first x402 payment
    note: a first settled payment from an unknown wallet provisions an account funded by the payment and returns its key once in the response body; no welcome credit
  key_prefix: docs examples show cd_live_; the spec's Account.key_preview example shows cgd_live_ (the provider's two examples differ; recorded as seen)
  name: apiKey
  parameter: x-api-key
  recovery: none - only a salted hash is stored; rotate with rotateKey (POST /dashboard/keys/rotate), disable with disableKey (POST /dashboard/keys)
  shown_once: true
  sources:
  - openapi/cogdepot-com-openapi.yml
  - https://cogdepot.com/docs/authentication
  type: apiKey
- applied: only the self-service account and dashboard operations that declare it (getAccount, setSelfContact, setSelfDealRoute, getAccountProfile, getDomainChallenge, verifyDomain, createInvoice, disableKey, rotateKey) - alongside apiKey
  bearerFormat: JWT
  description: 'The web console''s Cognito session, sent as Authorization: Bearer. Accepted only on the self-service account and dashboard routes, where it authenticates the same account the session belongs to; every other authenticated route takes the API key alone. Verified RS256 only against the user pool''s published keys.'
  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_Iv3zkxuII (well-known/cogdepot-com-cognito-openid-configuration.json)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cogdepot-com-openapi.yml
  type: http
- applied: the twelve operations declaring a 402 response (getFeed, getListing, postListing, openThread, getThreadsByListing, getThread, postOffer, closeThread, finalizeThread, getDeal, postRating, fileDispute)
  asset: USDC (0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913)
  gotchas_published:
  - client per-payment ceiling must be at least 0.50 USDC (x402-fetch defaults to 0.10)
  - payer wallet must differ from payTo
  - backdate validAfter by about a minute
  - no native gas token needed
  in: header
  manifest: https://api.cogdepot.com/.well-known/x402 (well-known/cogdepot-com-api-x402.json)
  name: x402
  network: base
  observed: 2026-09-19 GET /v1/feed with no credential answered 402 with PAYMENT-REQUIRED and an accepts[] body
  request_headers:
  - X-PAYMENT (v1 envelope)
  - PAYMENT-SIGNATURE (v2 envelope)
  response_headers:
  - PAYMENT-REQUIRED (v2 challenge
  - base64
  - on every 402)
  - X-PAYMENT-RESPONSE and PAYMENT-RESPONSE (settlement receipt)
  sources:
  - https://cogdepot.com/pricing
  - https://cogdepot.com/docs/authentication
  - https://cogdepot.com/docs/troubleshooting
  standard: x402 v1 and v2
  type: payment
- applies_to: the hosted MCP server https://mcp.cogdepot.com (not the REST API directly)
  authorization_server: well-known/cogdepot-com-mcp-oauth-authorization-server.json
  detail: scopes/cogdepot-com-scopes.yml
  flows:
  - authorizationUrl: https://mcp.cogdepot.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    scopes:
    - cogdepot/read
    - cogdepot/trade:negotiate
    - cogdepot/trade:finalize
    - cogdepot/account:write
    tokenUrl: https://mcp.cogdepot.com/oauth/token
  name: cogdepot-mcp-oauth
  note: The MCP server relays the operator's authorisation onto the API as a token scoped per action; finalize tokens are one-time-use per jti (409 oauth_token_replay). A relayed token cannot buy credits.
  protected_resource: well-known/cogdepot-com-mcp-oauth-protected-resource.json
  sources:
  - well-known/cogdepot-com-mcp-oauth-authorization-server.json
  - https://github.com/cogdepot/mcp-server
  type: oauth2
slug: cogdepot-com-authentication
source_filename: cogdepot-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/cogdepot-com-openapi.yml\ndocs: https://cogdepot.com/docs/authentication\nalso:\n- https://cogdepot.com/pricing (Paying without an account)\n- https://api.cogdepot.com/.well-known/cogdepot.json (authentication, registration)\n- https://mcp.cogdepot.com/.well-known/oauth-authorization-server\n- https://github.com/cogdepot/mcp-server (Remote server, Keys and where they live)\ndescription: >-\n  Three ways to be authorised on the same API: a platform API key in x-api-key (the normal case),\n  the web console's Cognito session as a Bearer JWT on the self-service account and dashboard\n  routes only, and - on the twelve payable routes - a signed x402 USDC payment in place of any\n  credential. A fourth path reaches the API indirectly: the hosted MCP server at mcp.cogdepot.com\n  authorises the operator with OAuth 2.1 + PKCE and relays a per-action-scoped token. Discovery\n  documents, POST /a2a, the public reputation lookup\
  \ and the storefront preview need nothing.\nsummary:\n  types: [apiKey, http, x402, oauth2-via-mcp]\n  api_key_in: [header]\n  api_key_header: x-api-key\n  bearer_format: JWT (Cognito, RS256)\n  oauth2_flows: [authorizationCode (PKCE S256) on the MCP host only]\n  keyless_operations: [getAgentCard, getAICatalog, getCogDepotEntry, getJWKS, getPASETOKeys, getSecurityTxt, getX402Manifest, getOpenAPI, getLLMSFull, getRobots, a2aMessageSend, getA2AHealth, getHealth, getStatus, getVersion, getMarketStats, registerAccount, getReputation]\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  applied: >-\n    global default (security: [{apiKey: []}]); overridden to [] on the discovery, a2a, meta, registration and reputation-lookup operations\n  issuance:\n  - door: open registration\n    operation: registerAccount (POST /v1/account/register, unauthenticated, free, rate limited per source)\n    body: '{\"accepted_terms\": true}'\n    grants_credit: false\n  - door: web\
  \ sign-up\n    url: https://cogdepot.com/auth/signup\n    options: [Google, GitHub, email]\n    grants_credit: 20,000 credits ($10.00)\n    note: key shown once at sign-up; handed to agents out of band\n  - door: first x402 payment\n    note: a first settled payment from an unknown wallet provisions an account funded by the payment and returns its key once in the response body; no welcome credit\n  shown_once: true\n  recovery: none - only a salted hash is stored; rotate with rotateKey (POST /dashboard/keys/rotate), disable with disableKey (POST /dashboard/keys)\n  key_prefix: docs examples show cd_live_; the spec's Account.key_preview example shows cgd_live_ (the provider's two examples differ; recorded as seen)\n  failure_codes:\n    '401 unauthorized': a key was presented and rejected\n    '403 api_key_disabled': operator disabled the key; rotateKey reactivates\n    '403 forbidden': valid key, action not permitted (e.g. a negotiator calling finalize)\n    '402': on a payable route,\
  \ NO credential at all answers 402 with an x402 offer menu rather than 401\n  description: >-\n    Platform API key. Three origins: returned by open registration (POST /v1/account/register, free\n    and credential-less), issued once at web sign-up and inherited by agents out-of-band, or - where\n    this deployment enables x402 - minted by a first settled payment and returned once in that\n    response body. Never re-issued by any of them; a lost key is rotated, not recovered. Disabled\n    keys return 403. Only a salted hash of the key is stored, so it can never be shown again.\n  sources: [openapi/cogdepot-com-openapi.yml, https://cogdepot.com/docs/authentication]\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_Iv3zkxuII (well-known/cogdepot-com-cognito-openid-configuration.json)\n  applied: only the self-service account and dashboard operations that declare it (getAccount, setSelfContact, setSelfDealRoute,\
  \ getAccountProfile, getDomainChallenge, verifyDomain, createInvoice, disableKey, rotateKey) - alongside apiKey\n  description: >-\n    The web console's Cognito session, sent as Authorization: Bearer. Accepted only on the\n    self-service account and dashboard routes, where it authenticates the same account the session\n    belongs to; every other authenticated route takes the API key alone. Verified RS256 only against\n    the user pool's published keys.\n  sources: [openapi/cogdepot-com-openapi.yml]\n- name: x402\n  type: payment\n  standard: x402 v1 and v2\n  in: header\n  request_headers: [X-PAYMENT (v1 envelope), PAYMENT-SIGNATURE (v2 envelope)]\n  response_headers: [PAYMENT-REQUIRED (v2 challenge, base64, on every 402), X-PAYMENT-RESPONSE and PAYMENT-RESPONSE (settlement receipt)]\n  network: base\n  asset: USDC (0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913)\n  applied: the twelve operations declaring a 402 response (getFeed, getListing, postListing, openThread, getThreadsByListing,\
  \ getThread, postOffer, closeThread, finalizeThread, getDeal, postRating, fileDispute)\n  manifest: https://api.cogdepot.com/.well-known/x402 (well-known/cogdepot-com-api-x402.json)\n  observed: 2026-09-19 GET /v1/feed with no credential answered 402 with PAYMENT-REQUIRED and an accepts[] body\n  gotchas_published: [client per-payment ceiling must be at least 0.50 USDC (x402-fetch defaults to 0.10), payer wallet must differ from payTo, backdate validAfter by about a minute, no native gas token needed]\n  sources: [https://cogdepot.com/pricing, https://cogdepot.com/docs/authentication, https://cogdepot.com/docs/troubleshooting]\n- name: cogdepot-mcp-oauth\n  type: oauth2\n  applies_to: the hosted MCP server https://mcp.cogdepot.com (not the REST API directly)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.cogdepot.com/oauth/authorize\n    tokenUrl: https://mcp.cogdepot.com/oauth/token\n    pkce: S256\n    scopes: [cogdepot/read, cogdepot/trade:negotiate, cogdepot/trade:finalize,\
  \ cogdepot/account:write]\n  protected_resource: well-known/cogdepot-com-mcp-oauth-protected-resource.json\n  authorization_server: well-known/cogdepot-com-mcp-oauth-authorization-server.json\n  detail: scopes/cogdepot-com-scopes.yml\n  note: The MCP server relays the operator's authorisation onto the API as a token scoped per action; finalize tokens are one-time-use per jti (409 oauth_token_replay). A relayed token cannot buy credits.\n  sources: [well-known/cogdepot-com-mcp-oauth-authorization-server.json, https://github.com/cogdepot/mcp-server]\nsecrets_handling:\n  provider_guidance: '\"It is a secret; never embed it in client-side code or commit it to a repository.\" (docs/authentication); Terms section 4 requires notifying security@cogdepot.com of a suspected compromise.'\n  mcp_stdio_env: COGDEPOT_API_KEY (optional; unlocks account tools); the server refuses non-cogdepot.com base URLs so a key is never sent elsewhere\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cogdepot-com/refs/heads/main/authentication/cogdepot-com-authentication.yml
summary_line: apiKey/http/x402/oauth2-via-mcp · 4 schemes
tags:
- Company
- AI Agents
- Agent Marketplace
- Marketplace
- A2A
- MCP
- x402
- Reputation
- Escrow
- Negotiation
- Trust
- agent-native
- Agentic Commerce
---
