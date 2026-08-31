---
api_key_in:
- query
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cometh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cometh secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cometh
provider_slug: cometh
scheme_count: 2
schemes:
- applies_to:
  - https://bundler.cometh.io/{chainId}
  - https://paymaster.cometh.io/{chainId}
  - https://paymaster.cometh.io/sponsored-address/{chainId}/
  - https://paymaster.cometh.io/sponsored-chain/{chainId}/
  audience: front-end (public)
  example_form: https://bundler.cometh.io/CHAIN_ID?apikey=API_KEY
  in: query
  name: apikey
  parameter: apikey
  source: https://docs.cometh.io/bundler/bundler-api
  type: apiKey
- applies_to:
  - https://api.4337.cometh.io/recovery/start
  - https://api.4337.cometh.io/recovery/start-with-shared
  - https://api.4337.cometh.io/recovery/finalize
  - https://paymaster.cometh.io/sponsored-address/ (POST)
  - https://paymaster.cometh.io/sponsored-chain/ (POST)
  audience: back-end (server-to-server)
  in: header
  name: apisecret
  note: Documented both as a request header (api.defaults.headers.common["apisecret"]) and, in one paymaster example, as a query parameter (?apisecret=API_SECRET) — the docs are inconsistent about placement for the write routes.
  parameter: apisecret
  source: https://docs.cometh.io/advanced/social-recovery
  type: apiKey
slug: cometh-authentication
source_filename: cometh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: https://docs.cometh.io/quick-start/getting-started\ndocs:\n- https://docs.cometh.io/quick-start/getting-started\n- https://docs.cometh.io/bundler/bundler-api\n- https://docs.cometh.io/paymaster/paymaster-api\n- https://docs.cometh.io/advanced/social-recovery\nnote: >-\n  Derived by hand from the documented request examples rather than from an OpenAPI: Cometh publishes no machine-readable\n  contract (see x-coverage in apis.yml), so derive-authentication.py had no spec to read. Two credentials are\n  documented, both project-scoped and both issued from the app.cometh.io dashboard: `apikey`, passed in the QUERY\n  STRING and explicitly described as safe for front-end use (\"It will be used in your front-end to authenticate public\n  API calls\"), and `apisecret`, passed as an HTTP HEADER and documented as back-end only (\"Recovery endpoints are\n  protected with an apisecret, indicating that requests should be done from your\
  \ backend for privacy concerns\"). There\n  is no OAuth 2.0, no OIDC, no bearer-token flow and no mTLS anywhere in the documentation — a full-text search of\n  docs.cometh.io/llms-full.txt returns zero occurrences of \"Bearer\", \"x-api-key\" or any OAuth endpoint.\nsummary:\n  types: [apiKey]\n  api_key_in: [query, header]\n  api_key_names: [apikey, apisecret]\n  oauth2_flows: []\n  oidc: false\n  mtls: false\n  gateway: Kong\n  key_issuance: dashboard\n  key_issuance_url: https://app.cometh.io\n  key_scope: per-project-per-chain\n  self_serve: partial\nschemes:\n- name: apikey\n  type: apiKey\n  in: query\n  parameter: apikey\n  audience: front-end (public)\n  applies_to:\n  - https://bundler.cometh.io/{chainId}\n  - https://paymaster.cometh.io/{chainId}\n  - https://paymaster.cometh.io/sponsored-address/{chainId}/\n  - https://paymaster.cometh.io/sponsored-chain/{chainId}/\n  example_form: https://bundler.cometh.io/CHAIN_ID?apikey=API_KEY\n  source: https://docs.cometh.io/bundler/bundler-api\n\
  - name: apisecret\n  type: apiKey\n  in: header\n  parameter: apisecret\n  audience: back-end (server-to-server)\n  applies_to:\n  - https://api.4337.cometh.io/recovery/start\n  - https://api.4337.cometh.io/recovery/start-with-shared\n  - https://api.4337.cometh.io/recovery/finalize\n  - https://paymaster.cometh.io/sponsored-address/ (POST)\n  - https://paymaster.cometh.io/sponsored-chain/ (POST)\n  note: >-\n    Documented both as a request header (api.defaults.headers.common[\"apisecret\"]) and, in one paymaster example, as a\n    query parameter (?apisecret=API_SECRET) — the docs are inconsistent about placement for the write routes.\n  source: https://docs.cometh.io/advanced/social-recovery\nenforcement_observed:\n- url: https://api.4337.cometh.io/\n  status: 401\n  body: '{\"message\":\"No API key found in request\"}'\n  note: Kong key-auth plugin rejects unauthenticated requests before routing; observed 2026-08-17.\n- url: https://paymaster.cometh.io/\n  status: 401\n  body: '{\"\
  message\":\"No API key found in request\"}'\n  note: Observed 2026-08-17.\n- url: https://bundler.cometh.io/openapi.json\n  status: 404\n  body: '{\"message\":\"no Route matched with those values\"}'\n  note: >-\n    The bundler host routes only the per-chain JSON-RPC paths; unmatched paths 404 at the gateway rather than 401,\n    which is how the absence of a discovery document was confirmed.\nend_user_authentication:\n  note: >-\n    Distinct from API authentication. End users do not hold a Cometh credential: the wallet owner is a WebAuthn/passkey\n    signer (or an external EOA / Magic / Web3Auth / Turnkey / Privy signer), and delegated authority is expressed\n    on-chain as ERC-7579 smart sessions (session keys) with sudo or action policies.\n  signers:\n  - passkey (WebAuthn, platform authenticator)\n  - EOA wallet (MetaMask, Phantom, ...)\n  - Magic\n  - Web3Auth\n  - Turnkey\n  - Privy\n  delegated_access: ERC-7579 smart sessions (session keys) with sudo / action policies\n  recovery:\
  \ social recovery via Safe delay module, 24h challenge window, apisecret-protected API\n  docs: https://docs.cometh.io/advanced/session-keys\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cometh/refs/heads/main/authentication/cometh-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Blockchain
- account-abstraction
- erc-4337
- smart-wallet
- paymaster
- bundler
- passkeys
- webauthn
- gasless-transactions
- DeFi
- custody
- staking
- Payments
- json-rpc
- mica
- safe
- Web3
---
