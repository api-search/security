---
anonymous_access: false
api_key_in: []
api_specs:
- filename: horizonshield-dev-mcp-conduct-register-openapi.json
  format: json
  label: MCP Verification Gate (MCP conduct register) API
  slug: mcp-verification-gate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizonshield-dev/refs/heads/main/openapi/horizonshield-dev-mcp-conduct-register-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Horizonshield Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: HORIZON SHIELD declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: HORIZON SHIELD
provider_slug: horizonshield-dev
scheme_count: 0
schemes: []
slug: horizonshield-dev-authentication
source_filename: horizonshield-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://mcp.horizonshield.dev/\nderived_from: openapi/horizonshield-dev-mcp-conduct-register-openapi.json\ndocs:\n- https://github.com/ogasurfproject-jpg/horizon-shield/blob/main/plugin/README.md\n- https://gate.horizonshield.dev/openapi.json\n- https://ledger.horizonshield.dev/llms.txt\nsummary: >-\n  Every public surface is anonymous by design and says so: the plugin README (\"Read-only, no API key\"), the gate\n  OpenAPI description (\"Read only. No account, no key, no fee.\"), the ledger security.txt (\"read-only and\n  unauthenticated by design\"), the JIDEC card (securitySchemes {}, security []). Verified live: initialize,\n  tools/list, prompts/list, tools/call get_agent_card and A2A message/send all succeeded with no credential on\n  mcp.horizonshield.dev; tools/list succeeded on gate., jidec., web., hearing. and femtech.; every REST route probed\n  on gate. and ledger. answered without a key. No OAuth/OIDC discovery\
  \ document exists on any host. The only keys in\n  the system are the PROVIDER's signing keys (JWKS, ES256) used to sign agent cards and receipts, and the\n  caller-side SHA-256 recomputation that replaces trust in the issuer.\nschemes: []\nscheme_count: 0\nanonymous_access:\n  mcp:\n  - {endpoint: 'https://mcp.horizonshield.dev/', auth: none, verified: 'initialize 200, tools/list 200 (15), prompts/list 200 (5), tools/call get_agent_card 200'}\n  - {endpoint: 'https://gate.horizonshield.dev/mcp', auth: none, verified: 'tools/list 200 (5)'}\n  - {endpoint: 'https://jidec.horizonshield.dev/mcp', auth: none, verified: 'tools/list 200 (4)'}\n  - {endpoint: 'https://web.horizonshield.dev/mcp', auth: none, verified: 'initialize 200, tools/list 200 (5)'}\n  - {endpoint: 'https://hearing.horizonshield.dev/mcp', auth: none, verified: 'initialize 200, tools/list 200 (6)'}\n  - {endpoint: 'https://femtech.horizonshield.dev/mcp', auth: none, verified: 'initialize 200, tools/list 200 (9)'}\n  a2a:\n\
  \  - {endpoint: 'https://mcp.horizonshield.dev/', auth: none, verified: message/send 200 -> completed Task}\n  rest:\n  - {base: 'https://gate.horizonshield.dev', auth: none, verified: '/spec, /register, /changes, /self, /health, /sweep/last, /watchlist, /nenrin/window, /ext/conduct/v1, /history all 200'}\n  - {base: 'https://ledger.horizonshield.dev', auth: none, verified: '/, /ledger, /witness, /paths, /agreement, /health, /cite/jidec:entry:5 all 200'}\nopenapi_security:\n  securitySchemes: null\n  security: null\n  note: The gate contract declares no security at all, which here is accurate rather than an omission; an explicit empty security [] would make the anonymity machine-readable.\nwrite_surfaces_and_gating:\n  - {surface: 'POST https://gate.horizonshield.dev/check', gate: none, note: 'Anyone can request a measurement of any public MCP endpoint; by default no tool is called on the target. allow_tool_call: true is \"only for a server you control\" — an honour-system instruction,\
  \ not an enforced credential.'}\n  - {surface: 'POST https://ledger.horizonshield.dev/witness', gate: none, note: 'Anyone may submit a witness walk under their own name; acceptance is mechanical schema checking; bundled daily.'}\n  - {surface: 'MCP tool create_ap2_fairness_attestation', gate: none, note: Appends a ledger record without any credential.}\n  - {surface: 'MCP tool register_source (femtech)', gate: none, note: 'Appends a registry entry after machine checks of five conditions.'}\n  - {surface: 'admin routes', gate: 'not public', note: 'The ledger''s privacy block names POST /ledger/append, POST /reference/pin and GET /ledger/pending as admin routes that are \"not measured at all\"; they were not probed.'}\nprovider_signing_keys:\n  jwks: well-known/horizonshield-dev-jwks.json\n  key: {kty: EC, crv: P-256, kid: hs-2026-09, alg: ES256, use: sig}\n  hosts_serving_it: [mcp.horizonshield.dev, gate.horizonshield.dev, ledger.horizonshield.dev, femtech.horizonshield.dev]\n  used_for:\n\
  \  - agent card signatures[] (JWS; jku -> that host's jwks.json)\n  - gate verdict records (record_sha256 recomputation)\n  - ledger claims\n  note: These authenticate the PROVIDER to the caller, not the caller to the provider.\nconsumer_web_products:\n  note: 'The human-facing products (EHN board, kantei appraisal) use LINE login and PayPal checkout on the docs site; the privacy policy says card data is held by PayPal. Out of scope for the API surface.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horizonshield-dev/refs/heads/main/authentication/horizonshield-dev-authentication.yml
summary_line: 0 schemes
tags:
- Construction
- Renovation
- Cost Estimation
- Fair Pricing
- Consumer Protection
- Verification
- Transparency Ledger
- Open Data
- MCP
- A2A
- AP2
- Agents
- Agent-Native
- Japan
---
