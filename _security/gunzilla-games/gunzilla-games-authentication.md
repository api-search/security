---
api_key_in: []
auth_types:
- none
- network-allowlist
- wallet-signature
description: ''
kind: authentication
layout: security
method: searched
name: Gunzilla Games Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gunzilla Games secures its APIs with none, network-allowlist, and wallet-signature across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gunzilla Games
provider_slug: gunzilla-games
scheme_count: 5
schemes:
- applies_to:
  - GUNZ Chain JSON-RPC API
  - GUNZScan Explorer API
  description: Read methods on the public GUNZ RPC node and every GUNZScan surface (REST v2, the Etherscan-compatible module/action API, and GraphQL) are served without any credential. Verified by anonymous HTTP requests returning 200 with real data.
  evidence:
  - POST https://rpc.gunzchain.io/ext/bc/2M47.../rpc {"method":"eth_chainId"} -> 200 {"result":"0xa99b"}
  - GET https://gunzscan.io/api/v2/stats -> 200 application/json
  - POST https://gunzscan.io/api/v1/graphql introspection -> 200
  name: anonymous-read
  type: none
- applies_to:
  - GUNZ Chain JSON-RPC API
  description: Gunzilla offers IP allow-listing on the public RPC endpoint for partners. This is an availability/rate-limit control obtained by contacting the team, not a per-request credential.
  name: network-allowlist
  quote: '"If you intend to utilize our RPC endpoint, please provide the IP addresses of your services so that we can whitelist them. This will eliminate potential limit hits."'
  request_channel: Contact the Gunzilla team via https://gunbygunz.com/develop/
  type: ip-allowlist
- algorithm: ECDSA secp256k1 (Ethereum / EIP-155 replay-protected)
  applies_to:
  - GUNZ Chain JSON-RPC API
  description: Writes are submitted as pre-signed raw transactions via eth_sendRawTransaction. The signing key is the caller's own EVM private key; the chain authenticates the recovered sender address. Chain ID 43419 is bound into the signature by EIP-155, so a GUNZ transaction cannot be replayed on another EVM chain.
  name: transaction-signature
  tooling: web3.js, ethers.js and standard Ethereum libraries, per the GUNZ documentation.
  type: wallet-signature
- applies_to:
  - GUNZ Chain JSON-RPC API
  description: GUNZ is a permissioned L1. A signed and otherwise valid contract-deployment transaction is rejected unless the sending address has been approved by Gunzilla. Validator participation is likewise restricted to approved partners and Ava Labs nodes.
  name: deployment-permission
  quote: '"our subnet is permissioned, meaning that you cannot deploy smart contracts without your addresses'' approval. If you wish to deploy your code, we will need a description of its purpose."'
  type: out-of-band-authorization
- applies_to:
  - api.gunztoken.io
  - marketplace.gunztoken.io
  description: api.gunztoken.io and marketplace.gunztoken.io answer HTTP 403 behind a Cloudflare bot challenge on every path except /.well-known/*, where the backend leaks a FastAPI-shaped {"detail":"Not Found"} body. No authentication scheme could be observed anonymously and none is documented publicly. Recorded as gated, not as absent.
  evidence:
  - GET https://api.gunztoken.io/openapi.json -> 403 (Cloudflare "Just a moment...")
  - GET https://api.gunztoken.io/llms.txt -> 404 application/json {"detail":"Not Found"}
  name: gunztoken-api-gate
  status: gated
  type: unknown
slug: gunzilla-games-authentication
source_filename: gunzilla-games-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://gunbygunz.com/documentation/\ndocs: https://gunbygunz.com/documentation/\nsummary:\n  types:\n  - none\n  - network-allowlist\n  - wallet-signature\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    Gunzilla publishes no API keys, no OAuth, and no token endpoint on its public surfaces. Every\n    public read surface answers anonymously. Write access is authenticated cryptographically at the\n    protocol layer (an ECDSA secp256k1 signature over the transaction by the sending EVM account),\n    not by an API credential. Privileged access - contract deployment, validator participation, and\n    the gunztoken.io marketplace/minting API - is granted out of band by the Gunzilla team.\nschemes:\n- name: anonymous-read\n  type: none\n  applies_to:\n  - GUNZ Chain JSON-RPC API\n  - GUNZScan Explorer API\n  description: >-\n    Read methods on the public GUNZ RPC node and every GUNZScan surface (REST v2, the\n    Etherscan-compatible\
  \ module/action API, and GraphQL) are served without any credential. Verified\n    by anonymous HTTP requests returning 200 with real data.\n  evidence:\n  - 'POST https://rpc.gunzchain.io/ext/bc/2M47.../rpc {\"method\":\"eth_chainId\"} -> 200 {\"result\":\"0xa99b\"}'\n  - GET https://gunzscan.io/api/v2/stats -> 200 application/json\n  - POST https://gunzscan.io/api/v1/graphql introspection -> 200\n- name: network-allowlist\n  type: ip-allowlist\n  applies_to:\n  - GUNZ Chain JSON-RPC API\n  description: >-\n    Gunzilla offers IP allow-listing on the public RPC endpoint for partners. This is an\n    availability/rate-limit control obtained by contacting the team, not a per-request credential.\n  quote: >-\n    \"If you intend to utilize our RPC endpoint, please provide the IP addresses of your services so\n    that we can whitelist them. This will eliminate potential limit hits.\"\n  request_channel: Contact the Gunzilla team via https://gunbygunz.com/develop/\n- name: transaction-signature\n\
  \  type: wallet-signature\n  algorithm: ECDSA secp256k1 (Ethereum / EIP-155 replay-protected)\n  applies_to:\n  - GUNZ Chain JSON-RPC API\n  description: >-\n    Writes are submitted as pre-signed raw transactions via eth_sendRawTransaction. The signing key\n    is the caller's own EVM private key; the chain authenticates the recovered sender address. Chain\n    ID 43419 is bound into the signature by EIP-155, so a GUNZ transaction cannot be replayed on\n    another EVM chain.\n  tooling: web3.js, ethers.js and standard Ethereum libraries, per the GUNZ documentation.\n- name: deployment-permission\n  type: out-of-band-authorization\n  applies_to:\n  - GUNZ Chain JSON-RPC API\n  description: >-\n    GUNZ is a permissioned L1. A signed and otherwise valid contract-deployment transaction is\n    rejected unless the sending address has been approved by Gunzilla. Validator participation is\n    likewise restricted to approved partners and Ava Labs nodes.\n  quote: >-\n    \"our subnet is permissioned,\
  \ meaning that you cannot deploy smart contracts without your\n    addresses' approval. If you wish to deploy your code, we will need a description of its purpose.\"\n- name: gunztoken-api-gate\n  type: unknown\n  applies_to:\n  - api.gunztoken.io\n  - marketplace.gunztoken.io\n  status: gated\n  description: >-\n    api.gunztoken.io and marketplace.gunztoken.io answer HTTP 403 behind a Cloudflare bot challenge\n    on every path except /.well-known/*, where the backend leaks a FastAPI-shaped\n    {\"detail\":\"Not Found\"} body. No authentication scheme could be observed anonymously and none is\n    documented publicly. Recorded as gated, not as absent.\n  evidence:\n  - GET https://api.gunztoken.io/openapi.json -> 403 (Cloudflare \"Just a moment...\")\n  - GET https://api.gunztoken.io/llms.txt -> 404 application/json {\"detail\":\"Not Found\"}\ngaps:\n- No developer signup, no API key issuance, no OAuth 2.0 or OpenID Connect anywhere on the public\n  surface.\n- The minting-engine and\
  \ marketplace APIs advertised on https://gunbygunz.com/develop/ have no\n  public authentication documentation; access is by application form only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gunzilla-games/refs/heads/main/authentication/gunzilla-games-authentication.yml
summary_line: none/network-allowlist/wallet-signature · 5 schemes
tags:
- Company
- Gaming
- Blockchain
- Web3
- EVM
- Avalanche
- JSON-RPC
- GraphQL
- Block Explorer
- NFT
- Video Games
---
