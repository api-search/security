---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: anyapi-gateway-openapi.json
  format: json
  label: AnyAPI Gateway API
  slug: anyapi-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anyapi/refs/heads/main/openapi/anyapi-gateway-openapi.json
auth_types:
- apiKey
- http
- oauth2
- inline-payment
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Anyapi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- deviceCode
overview: AnyAPI secures its APIs with apiKey, http, oauth2, and inline-payment across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and deviceCode flow(s).
provider_name: AnyAPI
provider_slug: anyapi
scheme_count: 6
schemes:
- description: Your AnyAPI key.
  in: header
  key_prefix: aa_live_
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/anyapi-gateway-openapi.json
  type: apiKey
- description: Your AnyAPI key as a Bearer token.
  key_prefix: aa_live_
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/anyapi-gateway-openapi.json
  type: http
- access_token_lifetime: about one hour, refreshed automatically by the first-party clients
  description: OAuth 2.1 with PKCE (S256) plus RFC 8628 device code, with open dynamic client registration and no client secret. The path hosted MCP clients (Claude, ChatGPT) take, and what `anyapi login` / `anyapi connect` drive from the CLI.
  detail: scopes/anyapi-scopes.yml
  flows:
  - authorizationUrl: https://api.getanyapi.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.getanyapi.com/oauth/token
  - deviceAuthorizationUrl: https://api.getanyapi.com/oauth/device_authorization
    flow: deviceCode
    tokenUrl: https://api.getanyapi.com/oauth/token
  - flow: refreshToken
    tokenUrl: https://api.getanyapi.com/oauth/token
  issuer: https://api.getanyapi.com
  name: OAuth2
  registration_endpoint: https://api.getanyapi.com/oauth/register
  revocation_endpoint: https://api.getanyapi.com/oauth/revoke
  scopes:
  - run
  - balance:read
  sources:
  - https://api.getanyapi.com/.well-known/oauth-authorization-server
  - https://api.getanyapi.com/.well-known/oauth-protected-resource
  token_prefix: aa_at_
  type: oauth2
- description: 'An unusual credential-issuance path worth recording: POST https://api.getanyapi.com/agent/signup with an optional {label} mints an aa_live_ trial key with no human, no email and no account. The secret is returned once, carries roughly $0.05 of requests, and self-expires in 7 days if never upgraded. Exhausting it returns HTTP 402 trial_cap_reached with a live RFC 8628 device authorization so the human can approve continued spend.'
  docs: https://getanyapi.com/docs/agent-self-signup
  name: AgentSelfSignup
  returns:
  - secret
  - keyId
  - capUsd
  - expiresAt
  - notice
  - clientId
  - upgrade
  sources:
  - https://getanyapi.com/.well-known/anyapi.json
  type: apiKey
- description: Pay per call with no account and no key. Call with no credential, receive HTTP 402 with a PAYMENT-REQUIRED header, sign and retry with PAYMENT-SIGNATURE (v2) or X-PAYMENT (v1). Settles in USDC on Base mainnet (eip155:8453); gasless, the facilitator sponsors gas. Settles AFTER execution, so a failed run never charges. The wallet is the identity.
  docs: https://getanyapi.com/docs/agent-payments
  name: x402
  receipt_headers:
  - PAYMENT-RESPONSE
  - X-PAYMENT-RESPONSE
  sources:
  - openapi/anyapi-gateway-openapi.json
  type: inline-payment
- description: Machine Payments Protocol on Tempo (chain id 4217). Call with no credential, receive a WWW-Authenticate:Payment challenge, settle on-chain and replay the credential in Authorization:Payment. Settles BEFORE execution; the provider states that if execution then fails the transfer cannot be automatically reversed.
  docs: https://getanyapi.com/docs/agent-payments
  name: mpp
  receipt_headers:
  - Payment-Receipt
  sources:
  - openapi/anyapi-gateway-openapi.json
  type: inline-payment
slug: anyapi-authentication
source_filename: anyapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: openapi/anyapi-gateway-openapi.json\ndocs: https://getanyapi.com/docs/api-keys\nupgraded_from: derived\nupgrade_note: >-\n  The derived pass read the two schemes the OpenAPI declares. The docs and the live discovery\n  documents add three more mechanisms the spec does not model at all - OAuth 2.1, autonomous\n  agent self-signup, and two inline crypto payment rails that authenticate a caller by wallet\n  rather than by credential - so the spec understates this API's auth surface considerably.\nsummary:\n  types: [apiKey, http, oauth2, inline-payment]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, refreshToken, deviceCode]\n  anonymous_surface: true\n  anonymous_note: >-\n    GET /catalog and GET /catalog/search require no credential at all, and MCP tools/list\n    answers 200 anonymously. Discovery is open; execution is gated.\nschemes:\n  - name: apiKeyAuth\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n\
  \    description: Your AnyAPI key.\n    key_prefix: aa_live_\n    sources: [openapi/anyapi-gateway-openapi.json]\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: Your AnyAPI key as a Bearer token.\n    key_prefix: aa_live_\n    sources: [openapi/anyapi-gateway-openapi.json]\n  - name: OAuth2\n    type: oauth2\n    description: >-\n      OAuth 2.1 with PKCE (S256) plus RFC 8628 device code, with open dynamic client\n      registration and no client secret. The path hosted MCP clients (Claude, ChatGPT) take,\n      and what `anyapi login` / `anyapi connect` drive from the CLI.\n    issuer: https://api.getanyapi.com\n    flows:\n      - {flow: authorizationCode, authorizationUrl: 'https://api.getanyapi.com/oauth/authorize', tokenUrl: 'https://api.getanyapi.com/oauth/token', pkce: S256}\n      - {flow: deviceCode, deviceAuthorizationUrl: 'https://api.getanyapi.com/oauth/device_authorization', tokenUrl: 'https://api.getanyapi.com/oauth/token'}\n      - {flow: refreshToken,\
  \ tokenUrl: 'https://api.getanyapi.com/oauth/token'}\n    registration_endpoint: https://api.getanyapi.com/oauth/register\n    revocation_endpoint: https://api.getanyapi.com/oauth/revoke\n    scopes: [run, 'balance:read']\n    token_prefix: aa_at_\n    access_token_lifetime: about one hour, refreshed automatically by the first-party clients\n    sources:\n      - https://api.getanyapi.com/.well-known/oauth-authorization-server\n      - https://api.getanyapi.com/.well-known/oauth-protected-resource\n    detail: scopes/anyapi-scopes.yml\n  - name: AgentSelfSignup\n    type: apiKey\n    description: >-\n      An unusual credential-issuance path worth recording: POST https://api.getanyapi.com/agent/signup\n      with an optional {label} mints an aa_live_ trial key with no human, no email and no\n      account. The secret is returned once, carries roughly $0.05 of requests, and self-expires\n      in 7 days if never upgraded. Exhausting it returns HTTP 402 trial_cap_reached with a live\n  \
  \    RFC 8628 device authorization so the human can approve continued spend.\n    returns: [secret, keyId, capUsd, expiresAt, notice, clientId, upgrade]\n    docs: https://getanyapi.com/docs/agent-self-signup\n    sources: [https://getanyapi.com/.well-known/anyapi.json]\n  - name: x402\n    type: inline-payment\n    description: >-\n      Pay per call with no account and no key. Call with no credential, receive HTTP 402 with a\n      PAYMENT-REQUIRED header, sign and retry with PAYMENT-SIGNATURE (v2) or X-PAYMENT (v1).\n      Settles in USDC on Base mainnet (eip155:8453); gasless, the facilitator sponsors gas.\n      Settles AFTER execution, so a failed run never charges. The wallet is the identity.\n    receipt_headers: [PAYMENT-RESPONSE, X-PAYMENT-RESPONSE]\n    docs: https://getanyapi.com/docs/agent-payments\n    sources: [openapi/anyapi-gateway-openapi.json]\n  - name: mpp\n    type: inline-payment\n    description: >-\n      Machine Payments Protocol on Tempo (chain id 4217). Call\
  \ with no credential, receive a\n      WWW-Authenticate:Payment challenge, settle on-chain and replay the credential in\n      Authorization:Payment. Settles BEFORE execution; the provider states that if execution\n      then fails the transfer cannot be automatically reversed.\n    receipt_headers: [Payment-Receipt]\n    docs: https://getanyapi.com/docs/agent-payments\n    sources: [openapi/anyapi-gateway-openapi.json]\ncredential_handling:\n  storage_guidance: >-\n    The provider's own llms.txt instructs agents to keep the key in the ANYAPI_API_KEY\n    environment variable, never in code.\n  cli_auth_order: ['--api-key flag', ANYAPI_API_KEY env, '~/.anyapi/config.json', trial self-signup]\n  spend_controls: Per-key limitUsd with daily/weekly/monthly reset windows, fixed expiry, reversible disable, permanent delete.\n  obtain_at: https://getanyapi.com/dashboard/keys\nrestrictions:\n  - Durable execution (Prefer:respond-async, GET /v1/requests/{id}) requires an authenticated wallet API\
  \ key and is NOT available on anonymous, x402 or MPP flows.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anyapi/refs/heads/main/authentication/anyapi-authentication.yml
summary_line: apiKey/http/oauth2/inline-payment · 6 schemes
tags:
- developer_tools
- data
- search
- scraping
- social_media
- ecommerce
- seo
- enrichment
- mcp
- agent-native
- web-data
- api-marketplace
- agent-payments
- x402
---
