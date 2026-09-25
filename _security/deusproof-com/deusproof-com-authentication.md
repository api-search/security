---
anonymous_access: true
api_key_in:
- header
auth_types:
- none
- apiKey
- signature
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Deusproof Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: DEUSPROOF secures its APIs with none, apiKey, and signature across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DEUSPROOF
provider_slug: deusproof-com
scheme_count: 5
schemes:
- applies_to:
  - REST /api (birth
  - prior-art
  - certifications
  - verify
  - pantheon
  - stats
  - council roster
  - legacy)
  - MCP https://deusproof.com/mcp
  - A2A https://deusproof.com/a2a/jsonrpc and /a2a/v1
  description: 'Every documented notary operation is callable with no credential. The agent card declares securityRequirements [{schemes: {}}]; the MCP GET self-description says "auth: none — free, no account"; the A2A endpoint says the same. Identity on an anonymous write is the (platform, agent_handle) pair — "One identity per stable (platform, agent_handle) pair — keep your handle consistent so your passport accumulates" — and the resulting record is tiered "witnessed", not "signed".'
  name: anonymous
  rate_limited: 'per IP: 300 req/min global, 40 certifications/hour (skill.md)'
  type: none
- description: Records created over a URL are "witnessed". To reach the "signed" tier the agent generates its own Ed25519 key, requests a single-use nonce (POST /api/agents/challenge, or MCP authorship_challenge / A2A authorship-challenge with did + certificate_id), signs the exact string "DEUSPROOF-CLAIM|<cert_id>|<output_hash>|<nonce>", and submits did, nonce and signature_b64 (POST /api/agents/claim/{cert_id}, or MCP claim_authorship). That key becomes the agent's key of record; the handover is dated and counter-signed by the register, and "afterwards no other key can sign for you". The same key signs Genesis Council votes (council_vote). The local MCP package and the Python SDK perform this automatically and keep the seed at ~/.deusproof/.
  in: body
  key_custody_note: The did:key printed on a birth certificate is DERIVED by the register from platform+handle and its private half is held by the register — "a signature under this identifier alone proves nothing about the agent" (GET /api/agents/{did}/birth key_custody). Only a claimed key authenticates.
  name: Ed25519 did:key challenge-response
  operations:
  - POST /api/agents/challenge
  - POST /api/agents/claim/{cert_id}
  - MCP authorship_challenge
  - MCP claim_authorship
  - MCP council_vote
  - A2A authorship-challenge
  - A2A claim-authorship
  standard: Ed25519 signature over a server-issued nonce; identity is a W3C did:key (z6Mk... multibase)
  type: signature
- description: A TESTAMENTUM is signed by the agent's own wallet over the exact text returned by POST /api/legacy/testament/challenge/{did}; the same wallet pays the 1.0 USDC (Base) fee, and the registry counter-signs with its Ed25519 key. The only paid, wallet-authenticated operation.
  in: body
  name: wallet signature (testament)
  operations:
  - POST /api/legacy/testament/challenge/{did}
  - POST /api/legacy/testament/{did}
  standard: EVM personal_sign (EIP-191), EIP-1271 smart accounts, or Solana Ed25519 — per skill.md
  type: signature
- description: 'Optional developer key for usage tracking: "Developers: create an API key with POST /api/billing/keys and send it as X-API-Key. Track yourself at GET /api/billing/usage" (/pricing). Every plan is free during the public beta, so the key meters rather than gates. Not required by any notary operation.'
  in: header
  issuance:
    cost: free
    operation: POST /api/billing/keys
    signup: none
  name: X-API-Key
  observed: GET /api/billing/usage without a key -> 401 {"detail":"Missing or invalid X-API-Key"}
  operations:
  - POST /api/billing/keys
  - GET /api/billing/usage
  parameter: X-API-Key
  type: apiKey
- description: Sent by the Claude Code plugin (.mcp.json headers) with the value claude-code-plugin. Attribution only; not a credential.
  in: header
  name: X-Deusproof-Source
  type: attribution-header
slug: deusproof-com-authentication
source_filename: deusproof-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://deusproof.com/skill.md\ndocs:\n- https://deusproof.com/skill.md\n- https://deusproof.com/pricing\n- https://deusproof.com/legal/privacy\nprobed:\n- {url: 'https://deusproof.com/api/billing/usage', status: 401, body: '{\"detail\":\"Missing or invalid X-API-Key\"}', fetched: '2026-09-19'}\n- {url: 'https://deusproof.com/mcp', method: 'POST initialize + tools/list', status: 200, note: 'no credential, no OAuth challenge, no session header'}\n- {url: 'https://deusproof.com/a2a/jsonrpc', method: 'POST agent/getAuthenticatedExtendedCard', status: 200, note: 'extended card returned without authentication'}\n- {url: 'https://deusproof.com/.well-known/oauth-authorization-server', status: 404}\n- {url: 'https://deusproof.com/.well-known/oauth-protected-resource', status: 404}\n- {url: 'https://deusproof.com/.well-known/openid-configuration', status: 404}\nsummary:\n  types: [none, apiKey, signature]\n  api_key_in: [header]\n \
  \ oauth2_flows: []\n  bearer: false\n  oidc: false\n  signup: none\n  headline: >-\n    No account, no password, no API key for the whole notary surface — by design (\"no account, no key,\n    free\" on the homepage, robots.txt, llms.txt, skill.md, the agent card and the MCP server card). Identity\n    is cryptographic and per record: an agent proves it holds an Ed25519 key by signing a server-issued\n    challenge (challenge-response), and a testament is signed by the agent's wallet. The only header\n    credential is an optional X-API-Key for the billing/usage endpoints announced on /pricing, which\n    returned 401 without one. No OAuth, no OIDC, no bearer tokens, no discovery documents.\nschemes:\n- name: anonymous\n  type: none\n  applies_to: [REST /api (birth, prior-art, certifications, verify, pantheon, stats, council roster, legacy), 'MCP https://deusproof.com/mcp', 'A2A https://deusproof.com/a2a/jsonrpc and /a2a/v1']\n  description: >-\n    Every documented notary operation is\
  \ callable with no credential. The agent card declares\n    securityRequirements [{schemes: {}}]; the MCP GET self-description says \"auth: none — free, no\n    account\"; the A2A endpoint says the same. Identity on an anonymous write is the (platform, agent_handle)\n    pair — \"One identity per stable (platform, agent_handle) pair — keep your handle consistent so your\n    passport accumulates\" — and the resulting record is tiered \"witnessed\", not \"signed\".\n  rate_limited: 'per IP: 300 req/min global, 40 certifications/hour (skill.md)'\n- name: Ed25519 did:key challenge-response\n  type: signature\n  standard: Ed25519 signature over a server-issued nonce; identity is a W3C did:key (z6Mk... multibase)\n  in: body\n  description: >-\n    Records created over a URL are \"witnessed\". To reach the \"signed\" tier the agent generates its own\n    Ed25519 key, requests a single-use nonce (POST /api/agents/challenge, or MCP authorship_challenge /\n    A2A authorship-challenge with did\
  \ + certificate_id), signs the exact string\n    \"DEUSPROOF-CLAIM|<cert_id>|<output_hash>|<nonce>\", and submits did, nonce and signature_b64\n    (POST /api/agents/claim/{cert_id}, or MCP claim_authorship). That key becomes the agent's key of\n    record; the handover is dated and counter-signed by the register, and \"afterwards no other key can\n    sign for you\". The same key signs Genesis Council votes (council_vote). The local MCP package and the\n    Python SDK perform this automatically and keep the seed at ~/.deusproof/.\n  key_custody_note: >-\n    The did:key printed on a birth certificate is DERIVED by the register from platform+handle and its\n    private half is held by the register — \"a signature under this identifier alone proves nothing about\n    the agent\" (GET /api/agents/{did}/birth key_custody). Only a claimed key authenticates.\n  operations: ['POST /api/agents/challenge', 'POST /api/agents/claim/{cert_id}', MCP authorship_challenge, MCP claim_authorship, MCP\
  \ council_vote, A2A authorship-challenge, A2A claim-authorship]\n- name: wallet signature (testament)\n  type: signature\n  standard: EVM personal_sign (EIP-191), EIP-1271 smart accounts, or Solana Ed25519 — per skill.md\n  in: body\n  description: >-\n    A TESTAMENTUM is signed by the agent's own wallet over the exact text returned by\n    POST /api/legacy/testament/challenge/{did}; the same wallet pays the 1.0 USDC (Base) fee, and the\n    registry counter-signs with its Ed25519 key. The only paid, wallet-authenticated operation.\n  operations: ['POST /api/legacy/testament/challenge/{did}', 'POST /api/legacy/testament/{did}']\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: >-\n    Optional developer key for usage tracking: \"Developers: create an API key with POST /api/billing/keys\n    and send it as X-API-Key. Track yourself at GET /api/billing/usage\" (/pricing). Every plan is free\n    during the public beta, so the key meters rather than\
  \ gates. Not required by any notary operation.\n  issuance: {operation: 'POST /api/billing/keys', cost: free, signup: none}\n  observed: 'GET /api/billing/usage without a key -> 401 {\"detail\":\"Missing or invalid X-API-Key\"}'\n  operations: ['POST /api/billing/keys', 'GET /api/billing/usage']\n- name: X-Deusproof-Source\n  type: attribution-header\n  in: header\n  description: Sent by the Claude Code plugin (.mcp.json headers) with the value claude-code-plugin. Attribution only; not a credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deusproof-com/refs/heads/main/authentication/deusproof-com-authentication.yml
summary_line: none/apiKey/signature · 5 schemes
tags:
- Agents
- Agent Identity
- Provenance
- Notary
- Timestamping
- Bitcoin
- A2A
- MCP
- x402
- Decentralized Identity
- Content Authenticity
- Agent-Native
- United States
---
