---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: getemboss-ai-account-openapi.yml
  format: yaml
  label: Emboss Account API
  slug: emboss-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getemboss-ai/refs/heads/main/openapi/getemboss-ai-account-openapi.yml
- filename: getemboss-ai-pay-per-call-openapi.yml
  format: yaml
  label: Emboss Pay-per-call API
  slug: emboss-pay-per-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getemboss-ai/refs/heads/main/openapi/getemboss-ai-pay-per-call-openapi.yml
auth_types:
- http
- oauth2
- payment
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Getemboss Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Emboss secures its APIs with http, oauth2, and payment across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Emboss
provider_slug: getemboss-ai
scheme_count: 6
schemes:
- bearerFormat: Emboss API key (sk_...)
  description: An Emboss API key. See https://getemboss.ai/docs/authentication.
  header: 'Authorization: Bearer sk_live_...'
  issuance: Created, rotated, disabled and revoked in the dashboard (Dashboard > Account > API keys); also the REST operations create_key_keys_post / list_keys_keys_get / patch_key_keys__key_id__patch / delete_key_keys__key_id__delete.
  key_prefix: sk_live_
  lifecycle:
    disabled: Requests return 401; reversible — re-enable in the dashboard.
    revoked: Requests return 401; permanent — issue a new key.
    rotation: Create the new key, move traffic, then revoke the old one.
    states:
    - active
    - disabled
    - revoked
  name: bearer
  rejections:
    401: No Authorization header or a malformed one; a well-formed but unknown, disabled or revoked key.
    402: Over the monthly free tier with no card on file.
    404: A valid key reaching a resource it does not own.
    429: Over the request rate limit.
  scheme: bearer
  scope: Owner-scoped — a key can only read and mutate the forms and sessions created with that same key; a request for another owner's resource returns 404, not 403, so existence is not leaked across accounts.
  sources:
  - openapi/getemboss-ai-account-openapi.yml
  - a2a/getemboss-ai-agent-card.json
  storage: Keys are stored hashed, never in plain text (https://getemboss.ai/security).
  test_mode: none — sk_live_ is the only prefix; see sandbox/getemboss-ai-sandbox.yml
  type: http
- consent: Dashboard shows pending consents and granted apps (admin_oauth_* operations); users disconnect under Dashboard > Account > Connected apps.
  description: Sign in with your Emboss account. See https://getemboss.ai/docs/authentication.
  detail: scopes/getemboss-ai-scopes.yml
  discovery: RFC 8414 metadata at https://api.getemboss.ai/.well-known/oauth-authorization-server; RFC 9728 metadata at https://api.getemboss.ai/.well-known/oauth-protected-resource/mcp
  flows:
  - authorizationUrl: https://api.getemboss.ai/oauth/authorize
    client_id_metadata_document_supported: true
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    registration_endpoint: https://api.getemboss.ai/oauth/register
    revocation_endpoint: https://api.getemboss.ai/oauth/revoke
    scopes: 2
    tokenUrl: https://api.getemboss.ai/oauth/token
    token_endpoint_auth_methods:
    - none
    - client_secret_post
  issuer: https://api.getemboss.ai
  name: oauth2
  sources:
  - openapi/getemboss-ai-account-openapi.yml
  - well-known/getemboss-ai-oauth-authorization-server.json
  - well-known/getemboss-ai-oauth-protected-resource-mcp.json
  - a2a/getemboss-ai-agent-card.json
  type: oauth2
  used_by:
  - MCP (https://api.getemboss.ai/mcp — 401 challenge carries resource_metadata)
  - A2A (card securitySchemes.oauth2)
  - account API (spec global security)
- applies_to: https://api.getemboss.ai/pay/* (openapi/getemboss-ai-pay-per-call-openapi.yml, x-payment-info.protocols[].mpp)
  challenge: '402 with WWW-Authenticate: Payment (one challenge per method: tempo USDC.e at the exact price; stripe card via Shared Payment Tokens with a 0.50 USD minimum)'
  docs: https://getemboss.ai/docs/pay-per-call/mpp
  name: payment-mpp
  note: An Authorization header that does not use the Payment scheme is answered with a fresh 402 rather than a 400.
  receipt: Payment-Receipt response header on the 202
  scheme: 'Authorization: Payment <credential>'
  type: payment
- applies_to:
  - https://api.getemboss.ai/pay/*
  - A2A tasks via the a2a-x402 extension (TASK_STATE_INPUT_REQUIRED with x402.payment.required)
  challenge: the same 402 carries a PAYMENT-REQUIRED header; accepts USDC on Base (eip155:8453) first, then one gasless GatewayWalletBatched entry per chain Circle Gateway supports
  docs: https://getemboss.ai/docs/pay-per-call/x402
  name: payment-x402
  note: Quotes expire after 24 hours; on A2A a failed attempt consumes the quote nonce, on the pay door a fresh 402 is issued.
  scheme: x402 payment header carrying a signed EIP-3009 TransferWithAuthorization
  type: payment
- description: Issued to anonymous pay-door callers with each result; proves ownership of an artifact so it can be reused in a later paid operation or a free utility without an account.
  docs: https://getemboss.ai/docs/artifacts
  location: request body, next to artifact_id (per source entry in sources[])
  name: artifact_token
  sources:
  - openapi/getemboss-ai-pay-per-call-openapi.yml (202 response artifact_token)
  type: capability-token
- description: HMAC(job_id, server secret) minted in the 202; lets an anonymous payer poll a job with no account.
  location: query parameter token on GET /pay/jobs/{job_id}
  name: status_url_token
  sources:
  - openapi/getemboss-ai-account-openapi.yml pay_job_status_pay_jobs__job_id__get description
  type: capability-token
slug: getemboss-ai-authentication
source_filename: getemboss-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/getemboss-ai-account-openapi.yml and openapi/getemboss-ai-pay-per-call-openapi.yml (derived baseline by derive-authentication.py) upgraded from https://getemboss.ai/docs/authentication, /docs/mcp-tools, /docs/a2a, /docs/pay-per-call/mpp, /docs/pay-per-call/x402, /docs/artifacts and the live discovery documents under well-known/\ndocs: https://getemboss.ai/docs/authentication\nsummary:\n  types: [http, oauth2, payment]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Four ways in, matched to four doors. (1) Bearer API key on the account REST API, A2A and (as a fallback) MCP.\n    (2) OAuth 2.1 authorization code + PKCE with dynamic client registration on MCP and A2A. (3) Machine payment\n    in place of identity on the anonymous pay door — an MPP \"Authorization: Payment\" credential or an x402\n    EIP-3009 authorization answering a 402. (4) artifact_token as a capability token that lets\
  \ an anonymous\n    caller reuse a file it paid for. GET /health and GET /library need nothing.\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: Emboss API key (sk_...)\n  header: 'Authorization: Bearer sk_live_...'\n  key_prefix: sk_live_\n  description: An Emboss API key. See https://getemboss.ai/docs/authentication.\n  sources: [openapi/getemboss-ai-account-openapi.yml, a2a/getemboss-ai-agent-card.json]\n  issuance: Created, rotated, disabled and revoked in the dashboard (Dashboard > Account > API keys); also the REST operations create_key_keys_post / list_keys_keys_get / patch_key_keys__key_id__patch / delete_key_keys__key_id__delete.\n  storage: Keys are stored hashed, never in plain text (https://getemboss.ai/security).\n  scope: Owner-scoped — a key can only read and mutate the forms and sessions created with that same key; a request for another owner's resource returns 404, not 403, so existence is not leaked across accounts.\n  lifecycle:\n    states:\
  \ [active, disabled, revoked]\n    disabled: Requests return 401; reversible — re-enable in the dashboard.\n    revoked: Requests return 401; permanent — issue a new key.\n    rotation: Create the new key, move traffic, then revoke the old one.\n  rejections:\n    401: No Authorization header or a malformed one; a well-formed but unknown, disabled or revoked key.\n    404: A valid key reaching a resource it does not own.\n    402: Over the monthly free tier with no card on file.\n    429: Over the request rate limit.\n  test_mode: none — sk_live_ is the only prefix; see sandbox/getemboss-ai-sandbox.yml\n- name: oauth2\n  type: oauth2\n  issuer: https://api.getemboss.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.getemboss.ai/oauth/authorize\n    tokenUrl: https://api.getemboss.ai/oauth/token\n    scopes: 2\n    pkce: S256\n    grant_types: [authorization_code, refresh_token]\n    registration_endpoint: https://api.getemboss.ai/oauth/register\n    revocation_endpoint:\
  \ https://api.getemboss.ai/oauth/revoke\n    token_endpoint_auth_methods: [none, client_secret_post]\n    client_id_metadata_document_supported: true\n  description: Sign in with your Emboss account. See https://getemboss.ai/docs/authentication.\n  sources: [openapi/getemboss-ai-account-openapi.yml, well-known/getemboss-ai-oauth-authorization-server.json, well-known/getemboss-ai-oauth-protected-resource-mcp.json, a2a/getemboss-ai-agent-card.json]\n  used_by: [MCP (https://api.getemboss.ai/mcp — 401 challenge carries resource_metadata), A2A (card securitySchemes.oauth2), account API (spec global security)]\n  discovery: RFC 8414 metadata at https://api.getemboss.ai/.well-known/oauth-authorization-server; RFC 9728 metadata at https://api.getemboss.ai/.well-known/oauth-protected-resource/mcp\n  consent: Dashboard shows pending consents and granted apps (admin_oauth_* operations); users disconnect under Dashboard > Account > Connected apps.\n  detail: scopes/getemboss-ai-scopes.yml\n- name:\
  \ payment-mpp\n  type: payment\n  scheme: 'Authorization: Payment <credential>'\n  challenge: '402 with WWW-Authenticate: Payment (one challenge per method: tempo USDC.e at the exact price; stripe card via Shared Payment Tokens with a 0.50 USD minimum)'\n  receipt: Payment-Receipt response header on the 202\n  applies_to: https://api.getemboss.ai/pay/* (openapi/getemboss-ai-pay-per-call-openapi.yml, x-payment-info.protocols[].mpp)\n  docs: https://getemboss.ai/docs/pay-per-call/mpp\n  note: An Authorization header that does not use the Payment scheme is answered with a fresh 402 rather than a 400.\n- name: payment-x402\n  type: payment\n  scheme: x402 payment header carrying a signed EIP-3009 TransferWithAuthorization\n  challenge: 'the same 402 carries a PAYMENT-REQUIRED header; accepts USDC on Base (eip155:8453) first, then one gasless GatewayWalletBatched entry per chain Circle Gateway supports'\n  applies_to: [https://api.getemboss.ai/pay/*, A2A tasks via the a2a-x402 extension (TASK_STATE_INPUT_REQUIRED\
  \ with x402.payment.required)]\n  docs: https://getemboss.ai/docs/pay-per-call/x402\n  note: Quotes expire after 24 hours; on A2A a failed attempt consumes the quote nonce, on the pay door a fresh 402 is issued.\n- name: artifact_token\n  type: capability-token\n  location: request body, next to artifact_id (per source entry in sources[])\n  description: Issued to anonymous pay-door callers with each result; proves ownership of an artifact so it can be reused in a later paid operation or a free utility without an account.\n  docs: https://getemboss.ai/docs/artifacts\n  sources: [openapi/getemboss-ai-pay-per-call-openapi.yml (202 response artifact_token)]\n- name: status_url_token\n  type: capability-token\n  location: query parameter token on GET /pay/jobs/{job_id}\n  description: HMAC(job_id, server secret) minted in the 202; lets an anonymous payer poll a job with no account.\n  sources: [openapi/getemboss-ai-account-openapi.yml pay_job_status_pay_jobs__job_id__get description]\npublic_endpoints:\n\
  - GET /health\n- GET /library\n- GET /pricing\n- POST /pay/quote\n- GET /.well-known/* discovery documents\nspec_gap: >-\n  The account spec declares bearer + oauth2 globally but the Idempotency-Key header, the payment schemes and the\n  artifact_token are documented only in prose; the pay spec declares security [] on each operation and expresses\n  payment through x-payment-info rather than a securityScheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getemboss-ai/refs/heads/main/authentication/getemboss-ai-authentication.yml
summary_line: http/oauth2/payment · 6 schemes
tags:
- PDF
- Forms
- Document Processing
- Form Filling
- Fax
- Data Extraction
- Agent-Native
- MCP
- A2A
- x402
- pay-per-call
- Government Forms
- Company
---
