---
api_key_in: []
auth_types:
- siwe
description: ''
kind: authentication
layout: security
method: searched
name: Lemon Cash Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lemon Cash secures its APIs with siwe across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lemon Cash
provider_slug: lemon-cash
scheme_count: 1
schemes:
- contract_wallets:
    erc6492: true
    note: Supports ERC-6492 so a user can authenticate before their smart-contract wallet is deployed; the wallet is deployed on the user's first transaction.
  description: The only supported authentication method for a Lemon Mini App. Presents the Mini App's Terms & Conditions, Privacy Policy and requested claims to the user inside the Lemon Cash app, then signs a SIWE message with the user's wallet and returns the wallet address, granted claims, signature and signed message.
  name: authenticate
  parameters:
  - description: EIP-155 chain id the authentication is bound to
    name: chainId
    required: true
    type: ChainId
  - description: Anti-replay nonce; must be at least 8 alphanumeric characters and generated server-side, one per attempt
    name: nonce
    required: false
    type: string
  - description: Claims requested from the user at consent time
    name: requirements.claims
    required: false
    type: ClaimKey[]
  returns:
  - description: The authenticated user's wallet address
    field: wallet
    type: string
  - description: Key/value pairs for the claims the user granted
    field: grantedClaims
    type: MiniAppGrantedClaim[]
  - description: SIWE signature proving wallet ownership
    field: signature
    type: string
  - description: The SIWE message that was signed
    field: message
    type: string
  sdk_function: authenticate
  sources:
  - https://lemoncash.mintlify.app/functions/authenticate
  standard: https://eips.ethereum.org/EIPS/eip-4361
  transport: react-native-webview postMessage bridge
  type: siwe
slug: lemon-cash-authentication
source_filename: lemon-cash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://lemoncash.mintlify.app/functions/authenticate\ndocs: https://lemoncash.mintlify.app/functions/authenticate\nnote: >-\n  Derived mechanically from OpenAPI securitySchemes was not possible — Lemon Cash\n  publishes no OpenAPI. The auth model below is captured verbatim from the Mini App\n  SDK documentation, which is the provider's only public developer contract.\nsummary:\n  types: [siwe]\n  standard: EIP-4361 Sign-In with Ethereum\n  api_key_in: []\n  oauth2_flows: []\n  bearer_tokens: false\n  api_keys: false\nschemes:\n- name: authenticate\n  type: siwe\n  standard: https://eips.ethereum.org/EIPS/eip-4361\n  transport: react-native-webview postMessage bridge\n  sdk_function: authenticate\n  sources: [https://lemoncash.mintlify.app/functions/authenticate]\n  description: >-\n    The only supported authentication method for a Lemon Mini App. Presents the\n    Mini App's Terms & Conditions, Privacy Policy and requested\
  \ claims to the user\n    inside the Lemon Cash app, then signs a SIWE message with the user's wallet and\n    returns the wallet address, granted claims, signature and signed message.\n  parameters:\n  - {name: chainId, type: ChainId, required: true, description: EIP-155 chain id the authentication is bound to}\n  - {name: nonce, type: string, required: false, description: 'Anti-replay nonce; must be at least 8 alphanumeric characters and generated server-side, one per attempt'}\n  - {name: requirements.claims, type: 'ClaimKey[]', required: false, description: Claims requested from the user at consent time}\n  returns:\n  - {field: wallet, type: string, description: The authenticated user's wallet address}\n  - {field: grantedClaims, type: 'MiniAppGrantedClaim[]', description: Key/value pairs for the claims the user granted}\n  - {field: signature, type: string, description: SIWE signature proving wallet ownership}\n  - {field: message, type: string, description: The SIWE message that\
  \ was signed}\n  contract_wallets:\n    erc6492: true\n    note: >-\n      Supports ERC-6492 so a user can authenticate before their smart-contract\n      wallet is deployed; the wallet is deployed on the user's first transaction.\nrules:\n- Call authenticate as soon as the user enters the Mini App, before deposit, withdraw,\n  transferMoney or callSmartContract.\n- Call authenticate on every entry so the wallet address is always fresh; re-trigger\n  when the user switches chains.\n- Generate the nonce in your backend, store it with an expiry and a used flag, and\n  verify it matches the nonce inside the signed message before trusting the signature.\n- Verify the SIWE signature server-side (the docs use viem verifySiweMessage, which\n  supports ERC-6492 contract wallets).\nconsent_claims:\n  model: user-granted claims requested at authentication time\n  docs: https://lemoncash.mintlify.app/types/types#claim-keys\n  claims:\n  - {key: NAME, description: The user's first name}\n  - {key:\
  \ LAST_NAME, description: The user's last name}\n  - {key: EMAIL, description: The user's email address}\n  - {key: IS_PEP, description: 'Whether the user is a Politically Exposed Person; Argentina only'}\n  - {key: LEMONTAG, description: The user's Lemon Cash tag (username)}\n  - {key: OPERATION_COUNTRY, description: The country where the user operates}\noauth2: false\noauth2_note: >-\n  No OAuth 2.0 or OpenID Connect surface. /.well-known/oauth-authorization-server and\n  /.well-known/openid-configuration both return 404 on lemon.me, so no scopes/\n  artifact was written — the ClaimKey set above is the consent surface instead.\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - {url: 'https://lemoncash.mintlify.app/functions/authenticate', http_status: 200}\n  - {url: 'https://lemoncash.mintlify.app/types/types', http_status: 200}\n  - {url: 'https://lemon.me/.well-known/openid-configuration', http_status: 404}\n  - {url: 'https://lemon.me/.well-known/oauth-authorization-server', http_status:\
  \ 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemon-cash/refs/heads/main/authentication/lemon-cash-authentication.yml
summary_line: siwe · 1 scheme
tags:
- Company
- Cryptocurrency
- Digital Wallet
- Fintech
- Payments
- Banking
- Blockchain
- Web3
- Argentina
- Latin America
- Mini Apps
- SDK
---
