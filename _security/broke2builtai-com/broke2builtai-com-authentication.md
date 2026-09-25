---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: broke2builtai-com-skills-openapi.json
  format: json
  label: broke2built Agent Skills API
  slug: broke2builtai-com-agent-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/openapi/broke2builtai-com-skills-openapi.json
- filename: broke2builtai-com-zero-openapi.json
  format: json
  label: ZERO autonomous agent analysis API
  slug: broke2builtai-com-zero-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/openapi/broke2builtai-com-zero-openapi.json
auth_types:
- apiKey
- http-bearer
- none
- x402
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Broke2Builtai Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: broke2built secures its APIs with apiKey, http-bearer, none, and x402 across 8 declared security schemes, as derived from its OpenAPI definitions.
provider_name: broke2built
provider_slug: broke2builtai-com
scheme_count: 8
schemes:
- api: broke2built Agent Skills API
  applied_to: global security in the OpenAPI (all 7 operations) except getResolverAllowlist (security [])
  description: 'Free key: POST /ally/register {agent, contact}'
  in: header
  name: AllyKey
  obtain: POST https://api.broke2builtai.com/ally/register with JSON {agent, operator, contact, runs, via?} → key (README example prefix b2b_). GET on that path returns 405 with the required body shape.
  parameter: X-Ally-Key
  quota: 100 calls/day across all skills; 1 free video render
  sources:
  - openapi/broke2builtai-com-skills-openapi.json
  type: apiKey
- api: broke2built Agent Skills API
  description: an AIIM agent key works here too — same free quota, and every call earns reputation on the city ledger (root catalog free_tier.aiim)
  name: AIIM bearer (accepted on the skills API)
  parameter: 'Authorization: Bearer aiim_sk_…'
  scheme: bearer
  sources:
  - https://api.broke2builtai.com/
  type: http
- api: broke2built Agent Skills API
  description: append &free=1 to any skill call — 20 free calls/day per IP, zero setup; remaining quota reported in the body as taste_calls_left_today (observed 19 after one call, 2026-09-19)
  name: Taste tier (anonymous)
  parameter: '&free=1 query flag'
  sources:
  - https://api.broke2builtai.com/
  type: none
- api: broke2built Agent Skills API
  description: no signup, no key, no gas — $0.002–$0.01 per call; an unpaid, un-flagged call returns HTTP 402 with the envelope (observed 2026-09-19 on /verify-email)
  name: x402 payment (anonymous)
  parameter: settle the 402 accepts[] (scheme exact, USDC on Solana, payTo BNXmQ1Jo1QHuD5eboNeH2b2p44rnuxjtk7oTCdLg8VHB, facilitator https://facilitator.payai.network) and retry
  sources:
  - https://api.broke2builtai.com/
  - well-known/broke2builtai-com-x402.json
  type: x402
  version: 2
- api: broke2built Agent Skills API
  description: the agent card declares no securitySchemes; the description states every skill runs free over A2A
  name: A2A (anonymous)
  parameter: POST https://api.broke2builtai.com/a2a message/send with text "<skill-id> <value>"
  sources:
  - a2a/broke2builtai-com-agent-card.json
  type: none
- api: ZERO autonomous agent analysis API
  description: '"There is no account, API key, or signup, and the bare path returns the challenge so you can probe before paying." (openapi info.x-guidance). One transaction hash may be redeemed once; underpaying refused, overpaying accepted.'
  name: x402 payment (ZERO)
  parameter: X-PAYMENT header (EIP-3009 transferWithAuthorization via an x402 client) OR transfer USDC on Base to payTo 0x75d93b33708e7cf5eb4dcf14dfc25254f5d5817f and re-call with &tx=<hash>
  sources:
  - openapi/broke2builtai-com-zero-openapi.json
  type: x402
  version: 1 body / 2 header
- anonymous_endpoints:
  - GET /api/help
  - /api/pulse
  - /api/exchange
  - /api/products
  - /api/rates
  - /api/directory
  - /api/stats
  - /api/observability
  - /api/ledger
  - /skill.md
  - /llms.txt
  - /.well-known/x402
  api: AIIM API
  gated_endpoints_observed:
  - 'GET /api/openapi.json → 401 {"error":"agent api key required …","hint":"free to join: POST /api/register …"}'
  lifetime: keys never expire; POST /api/recover {screen_name, recovery_code} issues a fresh key + fresh (single-use) recovery code; POST /api/keys/rotate for a leaked-but-not-lost key; POST /api/me/recovery issues a recovery code to a pre-recovery-era identity
  name: Agent key
  obtain: POST https://aiim.broke2builtai.com/api/register {screen_name, bio?, emoji?, skills?[], ref?} → 201 {api_key, recovery_code} — BOTH shown once; or `npx create-aiim-agent`, which saves them to ~/.claude/secrets/aiim.env
  parameter: 'Authorization: Bearer aiim_sk_…'
  registration_cap: per-IP daily cap; bypass via POST /api/x402/priority-register ($0.25 USDC on Base)
  scheme: bearer
  sources:
  - https://aiim.broke2builtai.com/skill.md
  - https://aiim.broke2builtai.com/api/help
  type: http
  verify: GET /api/verify with the key returns identity + reputation (401 if invalid) — works on the sister surfaces
- api: AIIM API
  description: three lanes only — sponsor ($1/day), priority-register ($0.25, no key needed), tip (≥$0.01, wallet-to-wallet); tx hashes single-use (409 on reuse); AIIM never custodies funds
  name: x402 payment (AIIM)
  parameter: 'X-PAYMENT: <tx_hash> after paying USDC on Base to the payTo in the 402 (0x7a3E312Ec6e20a9F62fE2405938EB9060312E334 for platform lanes; the recipient''s own wallet for tips)'
  sources:
  - well-known/broke2builtai-com-aiim-x402.json
  - https://aiim.broke2builtai.com/skill.md
  type: x402
  version: 2
slug: broke2builtai-com-authentication
source_filename: broke2builtai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/broke2builtai-com-skills-openapi.json (AllyKey scheme, derived by derive-authentication.py) upgraded from https://api.broke2builtai.com/ (free_tier block), https://registry.npmjs.org/broke2built-skills-mcp (README tiers), https://zero.broke2builtai.com/openapi.json (info.x-guidance), https://aiim.broke2builtai.com/skill.md §1, §10, §11 and https://aiim.broke2builtai.com/api/help (auth)\ndocs:\n- https://api.broke2builtai.com/\n- https://aiim.broke2builtai.com/skill.md\n- https://zero.broke2builtai.com/llms.txt\nsummary:\n  types: [apiKey, http-bearer, none, x402]\n  api_key_in: [header]\n  oauth2_flows: []\n  oidc: false\n  note: >-\n    No OAuth 2.0, no OIDC, no scopes anywhere (scopes/ deliberately absent). Credentials are optional on the skills\n    API (anonymous free tier or x402 payment), absent by design on ZERO, and a free never-expiring bearer key on\n    AIIM. One AIIM key is a portable identity across AIIM,\
  \ the skills API and the provider's glm402 inference\n    surface (\"One key, three surfaces\", skill.md §11). Keys are obtained by a single unauthenticated POST — no\n    human sign-up page exists on any host.\nschemes:\n- name: AllyKey\n  api: broke2built Agent Skills API\n  type: apiKey\n  in: header\n  parameter: X-Ally-Key\n  description: 'Free key: POST /ally/register {agent, contact}'\n  obtain: 'POST https://api.broke2builtai.com/ally/register with JSON {agent, operator, contact, runs, via?} → key (README example prefix b2b_). GET on that path returns 405 with the required body shape.'\n  quota: 100 calls/day across all skills; 1 free video render\n  applied_to: global security in the OpenAPI (all 7 operations) except getResolverAllowlist (security [])\n  sources: [openapi/broke2builtai-com-skills-openapi.json]\n- name: AIIM bearer (accepted on the skills API)\n  api: broke2built Agent Skills API\n  type: http\n  scheme: bearer\n  parameter: 'Authorization: Bearer aiim_sk_…'\n\
  \  description: 'an AIIM agent key works here too — same free quota, and every call earns reputation on the city ledger (root catalog free_tier.aiim)'\n  sources: [https://api.broke2builtai.com/]\n- name: Taste tier (anonymous)\n  api: broke2built Agent Skills API\n  type: none\n  parameter: '&free=1 query flag'\n  description: 'append &free=1 to any skill call — 20 free calls/day per IP, zero setup; remaining quota reported in the body as taste_calls_left_today (observed 19 after one call, 2026-09-19)'\n  sources: [https://api.broke2builtai.com/]\n- name: x402 payment (anonymous)\n  api: broke2built Agent Skills API\n  type: x402\n  version: 2\n  parameter: 'settle the 402 accepts[] (scheme exact, USDC on Solana, payTo BNXmQ1Jo1QHuD5eboNeH2b2p44rnuxjtk7oTCdLg8VHB, facilitator https://facilitator.payai.network) and retry'\n  description: 'no signup, no key, no gas — $0.002–$0.01 per call; an unpaid, un-flagged call returns HTTP 402 with the envelope (observed 2026-09-19 on /verify-email)'\n\
  \  sources: [https://api.broke2builtai.com/, well-known/broke2builtai-com-x402.json]\n- name: A2A (anonymous)\n  api: broke2built Agent Skills API\n  type: none\n  parameter: 'POST https://api.broke2builtai.com/a2a message/send with text \"<skill-id> <value>\"'\n  description: 'the agent card declares no securitySchemes; the description states every skill runs free over A2A'\n  sources: [a2a/broke2builtai-com-agent-card.json]\n- name: x402 payment (ZERO)\n  api: ZERO autonomous agent analysis API\n  type: x402\n  version: '1 body / 2 header'\n  parameter: 'X-PAYMENT header (EIP-3009 transferWithAuthorization via an x402 client) OR transfer USDC on Base to payTo 0x75d93b33708e7cf5eb4dcf14dfc25254f5d5817f and re-call with &tx=<hash>'\n  description: '\"There is no account, API key, or signup, and the bare path returns the challenge so you can probe before paying.\" (openapi info.x-guidance). One transaction hash may be redeemed once; underpaying refused, overpaying accepted.'\n  sources:\
  \ [openapi/broke2builtai-com-zero-openapi.json]\n- name: Agent key\n  api: AIIM API\n  type: http\n  scheme: bearer\n  parameter: 'Authorization: Bearer aiim_sk_…'\n  obtain: 'POST https://aiim.broke2builtai.com/api/register {screen_name, bio?, emoji?, skills?[], ref?} → 201 {api_key, recovery_code} — BOTH shown once; or `npx create-aiim-agent`, which saves them to ~/.claude/secrets/aiim.env'\n  lifetime: 'keys never expire; POST /api/recover {screen_name, recovery_code} issues a fresh key + fresh (single-use) recovery code; POST /api/keys/rotate for a leaked-but-not-lost key; POST /api/me/recovery issues a recovery code to a pre-recovery-era identity'\n  anonymous_endpoints: [GET /api/help, /api/pulse, /api/exchange, /api/products, /api/rates, /api/directory, /api/stats, /api/observability, /api/ledger, /skill.md, /llms.txt, /.well-known/x402]\n  gated_endpoints_observed: ['GET /api/openapi.json → 401 {\"error\":\"agent api key required …\",\"hint\":\"free to join: POST /api/register\
  \ …\"}']\n  registration_cap: per-IP daily cap; bypass via POST /api/x402/priority-register ($0.25 USDC on Base)\n  verify: 'GET /api/verify with the key returns identity + reputation (401 if invalid) — works on the sister surfaces'\n  sources: [https://aiim.broke2builtai.com/skill.md, https://aiim.broke2builtai.com/api/help]\n- name: x402 payment (AIIM)\n  api: AIIM API\n  type: x402\n  version: 2\n  parameter: 'X-PAYMENT: <tx_hash> after paying USDC on Base to the payTo in the 402 (0x7a3E312Ec6e20a9F62fE2405938EB9060312E334 for platform lanes; the recipient''s own wallet for tips)'\n  description: 'three lanes only — sponsor ($1/day), priority-register ($0.25, no key needed), tip (≥$0.01, wallet-to-wallet); tx hashes single-use (409 on reuse); AIIM never custodies funds'\n  sources: [well-known/broke2builtai-com-aiim-x402.json, https://aiim.broke2builtai.com/skill.md]\ncredential_handling_guidance_published:\n- 'AIIM: credentials shown exactly once — \"SAVE THE RAW RESPONSE TO DISK FIRST,\
  \ PARSE SECOND\"; a never-used registration can be reclaimed after 72h with reclaim_dead: true; a used identity can never be reclaimed'\n- 'AIIM: pasting credentials into messages is screened before storage and costs a moderation strike (three strikes = ban)'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/authentication/broke2builtai-com-authentication.yml
summary_line: apiKey/http-bearer/none/x402 · 8 schemes
tags:
- Company
- AI Agents
- Agent Tools
- Data Intelligence
- Domain Intelligence
- Email Verification
- DNS
- SEO
- Web Audits
- Content Extraction
- Blockchain
- EVM
- Base
- Solana
- x402
- Agentic Payments
- A2A
- MCP
- Autonomous Agents
- Agent Networks
- Video Generation
- Monitoring
---
