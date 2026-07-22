---
api_key_in: []
auth_types:
- web3-signed
- eip712-grants
- oauth2-oidc
description: ''
kind: authentication
layout: security
method: searched
name: Vana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vana secures its APIs with web3-signed, eip712-grants, and oauth2-oidc across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vana
provider_slug: vana
scheme_count: 4
schemes:
- description: Wallet-based request signing for the Personal Server REST API. The payload is alphabetically-sorted JSON with aud (server origin), method, uri, bodyHash, iat/exp timestamps, and grantId; the signature is EIP-191 over the base64url-encoded string, binding it to a specific server, method, and path.
  header: 'Authorization: Web3Signed <base64url(json)>.<signature>'
  name: Web3Signed
  scheme: web3-signed
  type: http
- description: 'Scope-native data-access permissions signed by the user''s wallet (domain "Vana Data Portability" version 2; message: grantor, granteeId, scopes[], expiresAt, nonce) and recorded onchain on Vana L1 (DataPortabilityPermissions). Verified on every request — existence, non-revocation, expiry, scope coverage, and fee payment.'
  name: EIP-712 grants (v2)
  type: grant
- description: ODL's optional commercial layer on top of the protocol offers OAuth/OIDC sign-in and USD billing — distinct from the protocol's RPC gateway.
  docs: https://docs.vana.org/applications/context-gateway
  name: Context Gateway OAuth/OIDC
  type: oauth2
- description: The protocol's authentication abstraction for users, builders, and Personal Servers (wallet-based identity; builder registration via DataPortabilityGrantees, server registration via DataPortabilityServers).
  docs: https://docs.vana.org/protocol-reference/identity
  name: Passport
  type: abstraction
slug: vana-authentication
source_filename: vana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.vana.org/protocol-reference/personal-servers\ndocs:\n  - https://docs.vana.org/protocol-reference/identity\n  - https://docs.vana.org/protocol-reference/grants-permissions\n  - https://docs.vana.org/applications/context-gateway\nsummary:\n  types: [web3-signed, eip712-grants, oauth2-oidc]\n  notes: >-\n    No OpenAPI securitySchemes exist to derive from; profile captured from the\n    protocol documentation.\nschemes:\n  - name: Web3Signed\n    type: http\n    scheme: web3-signed\n    header: 'Authorization: Web3Signed <base64url(json)>.<signature>'\n    description: >-\n      Wallet-based request signing for the Personal Server REST API. The\n      payload is alphabetically-sorted JSON with aud (server origin), method,\n      uri, bodyHash, iat/exp timestamps, and grantId; the signature is EIP-191\n      over the base64url-encoded string, binding it to a specific server,\n      method, and path.\n  - name: EIP-712\
  \ grants (v2)\n    type: grant\n    description: >-\n      Scope-native data-access permissions signed by the user's wallet\n      (domain \"Vana Data Portability\" version 2; message: grantor, granteeId,\n      scopes[], expiresAt, nonce) and recorded onchain on Vana L1\n      (DataPortabilityPermissions). Verified on every request — existence,\n      non-revocation, expiry, scope coverage, and fee payment.\n  - name: Context Gateway OAuth/OIDC\n    type: oauth2\n    description: >-\n      ODL's optional commercial layer on top of the protocol offers OAuth/OIDC\n      sign-in and USD billing — distinct from the protocol's RPC gateway.\n    docs: https://docs.vana.org/applications/context-gateway\n  - name: Passport\n    type: abstraction\n    description: >-\n      The protocol's authentication abstraction for users, builders, and\n      Personal Servers (wallet-based identity; builder registration via\n      DataPortabilityGrantees, server registration via DataPortabilityServers).\n\
  \    docs: https://docs.vana.org/protocol-reference/identity\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vana/refs/heads/main/authentication/vana-authentication.yml
summary_line: web3-signed/eip712-grants/oauth2-oidc · 4 schemes
tags:
- Company
- Crypto Ai
- Data Portability
- Personal Data
- Data Sovereignty
- Blockchain
- Web3
- Agents
- Artificial Intelligence
---
