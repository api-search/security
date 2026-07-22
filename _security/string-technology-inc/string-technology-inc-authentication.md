---
api_key_in:
- header
auth_types:
- apiKey
- walletSignature
- session
description: 'String uses two authentication layers: (1) API-key authentication for server-to-server and game-to-API calls via an X-Api-Key header, with two key classes — public keys (authenticate a game connecting to the String API) and secret keys (manage an organization programmatically); and (2) Web3 wallet-signature login for players (an EIP-4361 / Sign-In-With-Ethereum style challenge-response), where RequestToSign issues a nonce payload the player''s wallet signs, and the signed payload is verified to establish an authenticated session with refreshable auth cookies/tokens. Derived by hand from the docs because no machine-readable OpenAPI is publicly retrievable.'
kind: authentication
layout: security
method: searched
name: String Technology Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: String Technology Inc secures its APIs with apiKey, walletSignature, and session across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: String Technology Inc
provider_slug: string-technology-inc
scheme_count: 4
schemes:
- in: header
  key_class: public
  name: PublicApiKey
  parameter_name: X-Api-Key
  source: https://docs.string.xyz/docs/getting-started
  type: apiKey
  usage: Authenticates a game/client connecting to the String API. Safe for game-side use.
- in: header
  key_class: secret
  name: SecretApiKey
  parameter_name: X-Api-Key
  source: https://docs.string.xyz/docs/getting-started
  type: apiKey
  usage: Programmatic organization management. Must never be exposed in client-side code or public repos.
- flow:
    logout: POST /login/logout — invalidate the auth cookies
    refresh: POST /login/refresh — refresh the session token
    request_nonce: GET /login (RequestToSign) — returns a nonce payload for a given wallet address
    sign_and_verify: POST /login/sign — submit the signed noncePayload; String verifies the signature to authenticate the player
  name: WalletSignatureLogin
  source: https://docs.string.xyz/reference/get_login
  standard: EIP-4361 (Sign-In With Ethereum, challenge-response)
  type: walletSignature
- flow:
    login: POST /login — email/password login for organization members (dashboard)
    logout: POST /login/logout
    refresh: POST /login/refresh
  name: MemberLogin
  source: https://docs.string.xyz/reference/post_login
  type: session
slug: string-technology-inc-authentication
source_filename: string-technology-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.string.xyz/docs/basic-auth\ndocs:\n- https://docs.string.xyz/docs/basic-auth\n- https://docs.string.xyz/docs/integrated-auth\n- https://docs.string.xyz/docs/getting-started\ndescription: >-\n  String uses two authentication layers: (1) API-key authentication for\n  server-to-server and game-to-API calls via an X-Api-Key header, with two key\n  classes — public keys (authenticate a game connecting to the String API) and\n  secret keys (manage an organization programmatically); and (2) Web3\n  wallet-signature login for players (an EIP-4361 / Sign-In-With-Ethereum style\n  challenge-response), where RequestToSign issues a nonce payload the player's\n  wallet signs, and the signed payload is verified to establish an\n  authenticated session with refreshable auth cookies/tokens. Derived by hand\n  from the docs because no machine-readable OpenAPI is publicly retrievable.\nsummary:\n  types: [apiKey, walletSignature,\
  \ session]\n  api_key_in: [header]\n  api_key_header: X-Api-Key\nschemes:\n- name: PublicApiKey\n  type: apiKey\n  in: header\n  parameter_name: X-Api-Key\n  key_class: public\n  usage: Authenticates a game/client connecting to the String API. Safe for game-side use.\n  source: https://docs.string.xyz/docs/getting-started\n- name: SecretApiKey\n  type: apiKey\n  in: header\n  parameter_name: X-Api-Key\n  key_class: secret\n  usage: Programmatic organization management. Must never be exposed in client-side code or public repos.\n  source: https://docs.string.xyz/docs/getting-started\n- name: WalletSignatureLogin\n  type: walletSignature\n  standard: EIP-4361 (Sign-In With Ethereum, challenge-response)\n  flow:\n    request_nonce: GET /login (RequestToSign) — returns a nonce payload for a given wallet address\n    sign_and_verify: POST /login/sign — submit the signed noncePayload; String verifies the signature to authenticate the player\n    refresh: POST /login/refresh — refresh the session\
  \ token\n    logout: POST /login/logout — invalidate the auth cookies\n  source: https://docs.string.xyz/reference/get_login\n- name: MemberLogin\n  type: session\n  flow:\n    login: POST /login — email/password login for organization members (dashboard)\n    refresh: POST /login/refresh\n    logout: POST /login/logout\n  source: https://docs.string.xyz/reference/post_login\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/string-technology-inc/refs/heads/main/authentication/string-technology-inc-authentication.yml
summary_line: apiKey/walletSignature/session · 4 schemes
tags:
- Company
- Payments
- Web3
- Gaming
- Fiat On-Ramp
- Cryptocurrency
- NFT
- Merchant of Record
- Developer Tools
---
