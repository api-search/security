---
anonymous_access: true
api_key_in: []
auth_types:
- none
- erc8128-signed-request
- oauth2-metadata
description: Authentication profile for Name Whisper's agent surfaces. There is no OpenAPI, so this is read from the provider's own auth.md ("the authoritative source for how AI agents authenticate"), the RFC 8414 / RFC 9728 metadata documents it publishes, the ERC-8128 discovery document, and confirmed by live probes on 2026-09-19. The MCP and A2A endpoints are anonymous by default; ERC-8128 signed HTTP requests are the opt-in identity layer; no bearer tokens or API keys are ever issued.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Namewhisper Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: NameWhisper secures its APIs with none, erc8128-signed-request, and oauth2-metadata across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NameWhisper
provider_slug: namewhisper-ai
scheme_count: 4
schemes:
- description: All 44 tools are callable with no credential ("All 44 tools become available with no API key" - /guide). initialize, tools/list and an A2A message/send all succeeded anonymously. Unsigned callers get an anonymous result from get_caller_identity and no identity-aware features (reputation, usage tracking).
  name: anonymous
  probe:
    credentials: none
    method: POST tools/list
    status: 200
    url: https://namewhisper.ai/mcp
  surface: MCP https://namewhisper.ai/mcp and A2A https://namewhisper.ai/a2a
  type: none
- custody: none - transaction tools return unsigned transactions; the provider never holds keys
  description: 'Per-request cryptographic authentication: each HTTP request is signed by the caller''s Ethereum wallet (ERC-8128, https://erc8128.slice.so, EIP draft 8128). Accepted signing algorithms ES256K, EIP191 and EIP1271 (smart-contract wallets). Policy from the discovery document: maxValiditySec 300, replay protection via a nonce store, smart contract wallets supported. Signatures are verified per request and never exchanged for a bearer token. auth.md states write and transaction tools "require a signed request so the caller''s wallet is verifiable", while the discovery document and docs call ERC-8128 optional; live, the transaction tools return unsigned calldata for whatever walletAddress is passed, and it is the caller''s wallet that ultimately signs.'
  discovery: https://namewhisper.ai/.well-known/erc8128
  name: erc8128
  sources:
  - https://namewhisper.ai/.well-known/erc8128
  - https://namewhisper.ai/auth.md
  surface: MCP https://namewhisper.ai/mcp (and the REST twins under /api/*)
  type: erc8128-signed-request
- authorization_endpoint: https://namewhisper.ai/oauth/authorize
  description: 'RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata are published "for agent tooling that expects it", but the flows they describe are not standard OAuth: grant_types_supported is [erc8128_signed_request], response_types_supported is [none], token_endpoint_auth_methods_supported is [none, erc8128], and the note says "no bearer tokens are issued". The documents carry an agent_auth block whose register/claim/identity endpoints are all the MCP endpoint itself and whose registration tool is provision_agent_identity (an on-chain ENSIP-25 / ERC-8004 identity, not an OAuth client). /oauth/authorize and /oauth/token are named as endpoints but were not exercised.'
  files:
  - well-known/namewhisper-ai-oauth-authorization-server.json
  - well-known/namewhisper-ai-oauth-protected-resource.json
  issuer: https://namewhisper.ai
  name: oauth-metadata
  scopes:
  - mcp.read
  - mcp.transact
  surface: https://namewhisper.ai (issuer) for resource https://namewhisper.ai/mcp
  token_endpoint: https://namewhisper.ai/oauth/token
  type: oauth2-metadata
- description: The terms state "Authentication uses Sign-In with Ethereum (SIWE). Your account is tied to your Ethereum address" and the privacy policy that the session is a JWT in localStorage. This is the human web app's login, not an API credential, and is recorded for completeness.
  name: siwe
  sources:
  - https://namewhisper.ai/terms
  - https://namewhisper.ai/privacy
  surface: web app (namewhisper.ai) only
  type: sign-in-with-ethereum
slug: namewhisper-ai-authentication
source_filename: namewhisper-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource:\n- https://namewhisper.ai/auth.md\n- https://namewhisper.ai/.well-known/oauth-authorization-server\n- https://namewhisper.ai/.well-known/oauth-protected-resource\n- https://namewhisper.ai/.well-known/erc8128\n- https://namewhisper.ai/docs\n- https://namewhisper.ai/terms\ndocs: https://namewhisper.ai/auth.md\ndescription: >-\n  Authentication profile for Name Whisper's agent surfaces. There is no OpenAPI, so this is read from the\n  provider's own auth.md (\"the authoritative source for how AI agents authenticate\"), the RFC 8414 / RFC 9728\n  metadata documents it publishes, the ERC-8128 discovery document, and confirmed by live probes on 2026-09-19.\n  The MCP and A2A endpoints are anonymous by default; ERC-8128 signed HTTP requests are the opt-in identity\n  layer; no bearer tokens or API keys are ever issued.\nsummary:\n  types: [none, erc8128-signed-request, oauth2-metadata]\nschemes:\n- name: anonymous\n  type: none\n\
  \  surface: MCP https://namewhisper.ai/mcp and A2A https://namewhisper.ai/a2a\n  description: >-\n    All 44 tools are callable with no credential (\"All 44 tools become available with no API key\" - /guide).\n    initialize, tools/list and an A2A message/send all succeeded anonymously. Unsigned callers get an anonymous\n    result from get_caller_identity and no identity-aware features (reputation, usage tracking).\n  probe: {url: 'https://namewhisper.ai/mcp', method: POST tools/list, status: 200, credentials: none}\n- name: erc8128\n  type: erc8128-signed-request\n  surface: MCP https://namewhisper.ai/mcp (and the REST twins under /api/*)\n  description: >-\n    Per-request cryptographic authentication: each HTTP request is signed by the caller's Ethereum wallet\n    (ERC-8128, https://erc8128.slice.so, EIP draft 8128). Accepted signing algorithms ES256K, EIP191 and EIP1271\n    (smart-contract wallets). Policy from the discovery document: maxValiditySec 300, replay protection via a\
  \ nonce\n    store, smart contract wallets supported. Signatures are verified per request and never exchanged for a bearer\n    token. auth.md states write and transaction tools \"require a signed request so the caller's wallet is\n    verifiable\", while the discovery document and docs call ERC-8128 optional; live, the transaction tools return\n    unsigned calldata for whatever walletAddress is passed, and it is the caller's wallet that ultimately signs.\n  discovery: https://namewhisper.ai/.well-known/erc8128\n  custody: none - transaction tools return unsigned transactions; the provider never holds keys\n  sources: [https://namewhisper.ai/.well-known/erc8128, https://namewhisper.ai/auth.md]\n- name: oauth-metadata\n  type: oauth2-metadata\n  surface: https://namewhisper.ai (issuer) for resource https://namewhisper.ai/mcp\n  description: >-\n    RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata are published \"for agent\n    tooling that expects it\", but\
  \ the flows they describe are not standard OAuth: grant_types_supported is\n    [erc8128_signed_request], response_types_supported is [none], token_endpoint_auth_methods_supported is\n    [none, erc8128], and the note says \"no bearer tokens are issued\". The documents carry an agent_auth block\n    whose register/claim/identity endpoints are all the MCP endpoint itself and whose registration tool is\n    provision_agent_identity (an on-chain ENSIP-25 / ERC-8004 identity, not an OAuth client). /oauth/authorize\n    and /oauth/token are named as endpoints but were not exercised.\n  issuer: https://namewhisper.ai\n  authorization_endpoint: https://namewhisper.ai/oauth/authorize\n  token_endpoint: https://namewhisper.ai/oauth/token\n  scopes: [mcp.read, mcp.transact]\n  files:\n  - well-known/namewhisper-ai-oauth-authorization-server.json\n  - well-known/namewhisper-ai-oauth-protected-resource.json\n- name: siwe\n  type: sign-in-with-ethereum\n  surface: web app (namewhisper.ai) only\n  description:\
  \ >-\n    The terms state \"Authentication uses Sign-In with Ethereum (SIWE). Your account is tied to your Ethereum\n    address\" and the privacy policy that the session is a JWT in localStorage. This is the human web app's login,\n    not an API credential, and is recorded for completeness.\n  sources: [https://namewhisper.ai/terms, https://namewhisper.ai/privacy]\noauth: metadata-only\nopenid_connect: false\napi_keys: false\nnotes: >-\n  /.well-known/openid-configuration returns 404 - the issuer publishes RFC 8414 metadata but is not an OpenID\n  Provider. No API-key scheme exists anywhere. The scopes mcp.read and mcp.transact are recorded in\n  scopes/namewhisper-ai-scopes.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/namewhisper-ai/refs/heads/main/authentication/namewhisper-ai-authentication.yml
summary_line: none/erc8128-signed-request/oauth2-metadata · 4 schemes
tags:
- ENS
- Ethereum
- Web3
- Domain Names
- AI Agents
- MCP
- A2A
- Valuation
- NFT Marketplace
- Agent Identity
- Blockchain
---
