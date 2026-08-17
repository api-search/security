---
api_key_in:
- header
api_specs:
- filename: gala-games-galachain-asset-token-contract-openapi.json
  format: json
  label: GalaChain Token Contract API
  slug: galachain-token-contract
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gala-games/refs/heads/main/openapi/gala-games-galachain-asset-token-contract-openapi.json
- filename: gala-games-galachain-asset-dexv3-contract-openapi.json
  format: json
  label: GalaChain DEX v3 Contract API
  slug: galachain-dexv3-contract
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gala-games/refs/heads/main/openapi/gala-games-galachain-asset-dexv3-contract-openapi.json
- filename: gala-games-galachain-asset-launchpad-contract-openapi.json
  format: json
  label: GalaChain Launchpad Contract API
  slug: galachain-launchpad-contract
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gala-games/refs/heads/main/openapi/gala-games-galachain-asset-launchpad-contract-openapi.json
- filename: gala-games-galachain-asset-fee-contract-openapi.json
  format: json
  label: GalaChain Fee Contract API
  slug: galachain-fee-contract
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gala-games/refs/heads/main/openapi/gala-games-galachain-asset-fee-contract-openapi.json
- filename: gala-games-galachain-asset-public-key-contract-openapi.json
  format: json
  label: GalaChain Public Key Contract API
  slug: galachain-public-key-contract
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gala-games/refs/heads/main/openapi/gala-games-galachain-asset-public-key-contract-openapi.json
- filename: gala-games-galaconnect-openapi.json
  format: json
  label: GalaConnect API
  slug: galaconnect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gala-games/refs/heads/main/openapi/gala-games-galaconnect-openapi.json
- filename: gala-games-block-explorer-openapi.json
  format: json
  label: Gala Block Explorer API
  slug: block-explorer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gala-games/refs/heads/main/openapi/gala-games-block-explorer-openapi.json
- filename: gala-games-defi-backend-openapi.json
  format: json
  label: Gala DeFi Backend API
  slug: defi-backend
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gala-games/refs/heads/main/openapi/gala-games-defi-backend-openapi.json
auth_types:
- signature
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Gala Games Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gala Games secures its APIs with signature and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gala Games
provider_slug: gala-games
scheme_count: 4
schemes:
- algorithm: secp256k1
  applies_to:
  - GalaChain Gateway (all submit operations across all channels and contracts)
  - GalaConnect API (all write operations)
  fields:
  - description: Signature of the DTO signed with the caller's private key, verified against the public key saved on chain. Optional on the DTO type, required for a transaction to execute.
    name: signature
    required: for execution
  - base64 encoded.: null
    description: Public key of the signer
    name: signerPublicKey
    required: conditional
  - description: Address of the signer — typically an Ethereum address, or a user alias.
    name: signerAddress
    required: for multisig
  - description: Array of signatures when there are multiple signers. minItems 2. When present, signerAddress is required and signature/signerPublicKey are forbidden; the signing scheme must be ETH.
    name: multisig
    required: false
  - description: Prefix for MetaMask transaction signatures
    name: prefix
    needed to format payloads so publicKey can be recovered from web3 signatures.: null
    required: false
  - description: Idempotency key written to chain state; prevents double execution.
    name: uniqueKey
    required: true
  - description: Unix epoch milliseconds after which the DTO is invalid. Bounds replay exposure.
    name: dtoExpiresAt
    required: false
  - description: Full on-chain operation identifier in the form channelId_chaincodeId_methodName. Required for multisig DTOs, optional for single-signed ones.
    name: dtoOperation
    required: for multisig
  location: request body
  name: galachain-dto-signature
  procedure:
  - Remove any existing signature property from the body.
  - Recursively order every property alphabetically by name.
  - Stringify to a minimal deterministic JSON string.
  - keccak256 hash the stringified object.
  - Sign the hash with the wallet private key using secp256k1.
  - Normalize s to be less than or equal to half the curve order n.
  - DER encode and base64 the result; place it in the body as `signature`.
  reference_implementation: Published in full as TypeScript in the GalaConnect API description, and implemented in @gala-chain/api. `galachain dto:sign` performs the same operation from the CLI.
  type: signature
  verification_aid: Gala publishes worked examples whose signatures are genuinely correct for the documented example key, so an integrator can validate their signing code offline before ever calling the API.
- applies_to:
  - GalaConnect API
  description: Identifies the calling wallet on every GalaConnect write. Not a secret and not a credential on its own — it must be accompanied by a valid signature over the body. Format is client|<24 hex> for a Gala platform account or eth|<40 hex> for a headless or web3 wallet.
  in: header
  name: X-Wallet-Address
  parameter: X-Wallet-Address
  type: apiKey
- applies_to:
  - Gala DeFi Backend API
  description: Required for admin endpoints protected by ApiKeyGuard.
  in: header
  name: api-key
  note: The only securityScheme declared in any Gala OpenAPI document. Not obtainable by a public developer; there is no key-issuance flow published.
  parameter: X-Api-Key
  sources:
  - openapi/gala-games-defi-backend-openapi.json
  type: apiKey
- applies_to:
  - Gala Block Explorer API (all 17 operations)
  - GalaChain Gateway evaluate/read operations
  - GalaConnect read operations (swap discovery, GetPublicKey, /fee quotes)
  - Gala DeFi Backend public trade, explore, market, leaderboard and pairs endpoints
  description: A large, genuinely open read surface. An agent can read chain state, pool data, prices and swap inventory with no credential at all.
  name: none
  type: none
slug: gala-games-authentication
source_filename: gala-games-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: searched\nsource: https://connect.gala.com/info/swagger.json (info.description, Authentication +\n  Request Signing) + https://raw.githubusercontent.com/GalaChain/sdk/main/docs/authorization.md\n  + openapi/gala-games-defi-backend-openapi.json\ndocs: https://docs.galachain.com/latest/authorization/\nsummary:\n  types: [signature, apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  headline: >-\n    Gala's public APIs use NO bearer tokens, NO OAuth and NO OIDC. Reads are almost\n    entirely unauthenticated. Writes are authenticated by a secp256k1 signature over\n    the request body, verified against a public key registered on chain. The only\n    declared securityScheme across 413 published operations is one apiKey guarding\n    admin endpoints on the DeFi backend — the signature scheme that protects everything\n    that matters is documented in prose and modelled in no spec.\nschemes:\n- name: galachain-dto-signature\n  type: signature\n\
  \  algorithm: secp256k1\n  location: request body\n  applies_to:\n  - GalaChain Gateway (all submit operations across all channels and contracts)\n  - GalaConnect API (all write operations)\n  fields:\n  - {name: signature, required: for execution, description: 'Signature of the DTO signed\n      with the caller''s private key, verified against the public key saved on chain.\n      Optional on the DTO type, required for a transaction to execute.'}\n  - {name: signerPublicKey, required: conditional, description: Public key of the signer,\n      base64 encoded.}\n  - {name: signerAddress, required: for multisig, description: 'Address of the signer —\n      typically an Ethereum address, or a user alias.'}\n  - {name: multisig, required: false, description: 'Array of signatures when there are\n      multiple signers. minItems 2. When present, signerAddress is required and\n      signature/signerPublicKey are forbidden; the signing scheme must be ETH.'}\n  - {name: prefix, required: false,\
  \ description: Prefix for MetaMask transaction\n      signatures, needed to format payloads so publicKey can be recovered from web3\n      signatures.}\n  - {name: uniqueKey, required: true, description: 'Idempotency key written to chain\n      state; prevents double execution.'}\n  - {name: dtoExpiresAt, required: false, description: Unix epoch milliseconds after\n      which the DTO is invalid. Bounds replay exposure.}\n  - {name: dtoOperation, required: for multisig, description: 'Full on-chain operation\n      identifier in the form channelId_chaincodeId_methodName. Required for multisig\n      DTOs, optional for single-signed ones.'}\n  procedure:\n  - Remove any existing signature property from the body.\n  - Recursively order every property alphabetically by name.\n  - Stringify to a minimal deterministic JSON string.\n  - keccak256 hash the stringified object.\n  - Sign the hash with the wallet private key using secp256k1.\n  - Normalize s to be less than or equal to half the curve\
  \ order n.\n  - DER encode and base64 the result; place it in the body as `signature`.\n  reference_implementation: Published in full as TypeScript in the GalaConnect API\n    description, and implemented in @gala-chain/api. `galachain dto:sign` performs the\n    same operation from the CLI.\n  verification_aid: Gala publishes worked examples whose signatures are genuinely\n    correct for the documented example key, so an integrator can validate their signing\n    code offline before ever calling the API.\n- name: X-Wallet-Address\n  type: apiKey\n  in: header\n  parameter: X-Wallet-Address\n  applies_to: [GalaConnect API]\n  description: >-\n    Identifies the calling wallet on every GalaConnect write. Not a secret and not a\n    credential on its own — it must be accompanied by a valid signature over the body.\n    Format is client|<24 hex> for a Gala platform account or eth|<40 hex> for a headless\n    or web3 wallet.\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n\
  \  description: Required for admin endpoints protected by ApiKeyGuard.\n  applies_to: [Gala DeFi Backend API]\n  sources: [openapi/gala-games-defi-backend-openapi.json]\n  note: The only securityScheme declared in any Gala OpenAPI document. Not obtainable\n    by a public developer; there is no key-issuance flow published.\n- name: none\n  type: none\n  applies_to:\n  - Gala Block Explorer API (all 17 operations)\n  - GalaChain Gateway evaluate/read operations\n  - GalaConnect read operations (swap discovery, GetPublicKey, /fee quotes)\n  - Gala DeFi Backend public trade, explore, market, leaderboard and pairs endpoints\n  description: A large, genuinely open read surface. An agent can read chain state,\n    pool data, prices and swap inventory with no credential at all.\ncredential_acquisition:\n- path: Gala platform account\n  steps:\n  - Create an account at games.gala.com.\n  - Create a GalaChain transfer code at account settings, which initializes the wallet.\n  - Download the private\
  \ key from account settings (the docs expose a &plaintext query\n    parameter for advanced users).\n  - Retrieve the public key via POST /galachain/api/asset/public-key-contract/GetPublicKey\n    with your wallet address.\n  note: The key material is a wallet private key with spending authority, not a scoped\n    API credential. There is no way to issue a read-only or least-privilege token.\n- path: headless wallet\n  steps:\n  - Generate an ethers keypair locally.\n  - POST /v1/CreateHeadlessWallet with the public key in lowercase hex prefixed 0x\n    (note this differs from the base64 encoding used everywhere else in the API).\n  - Use address form eth|<address without 0x> as X-Wallet-Address.\n  note: No Gala platform account required. Headless and web3 wallets are interchangeable\n    with both the API and the website client.\n- path: on-chain key registration\n  contract: public-key-contract\n  note: A public key must be registered on chain before signatures from it verify.\nroles:\n\
  \  model: contract-level role annotations\n  observed: >-\n    Every gateway operation description carries an allowed-roles annotation, e.g.\n    \"Transaction is read only (evaluate). Allowed roles: EVALUATE.\" Roles seen across\n    the specs include EVALUATE, SUBMIT and CURATOR.\n  note: Roles are described per operation in the spec description text, not modelled as\n    OAuth scopes or as a securityScheme. There is no scopes surface to derive — see\n    scopes/ (intentionally absent).\noauth_scopes:\n  applicable: false\n  reason: No OAuth or OIDC anywhere. derive-oauth-scopes.py returned zero oauth2 schemes\n    across all nine specs.\ngaps:\n- The signature scheme is not modelled as an OpenAPI securityScheme on any of the 413\n  operations it protects, so generated SDKs and agent tooling see an unauthenticated\n  API and will produce calls that fail at 401.\n- Credentials are raw wallet private keys with full spending authority. There is no\n  scoped, revocable, least-privilege credential\
  \ for an integration or an agent, which\n  is why the MCP server's only safety control is \"omit PRIVATE_KEY for read-only mode\".\n- The private-key download flow instructs users to fetch plaintext key material over a\n  URL query parameter.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gala-games/refs/heads/main/authentication/gala-games-authentication.yml
summary_line: signature/apiKey · 4 schemes
tags:
- Company
- Blockchain
- Web3
- Gaming
- NFT
- Tokens
- DeFi
- Cryptocurrency
- Distributed Ledger
- Smart Contracts
- Entertainment
- Decentralized Exchange
---
