---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aelf-inc-node-web-api-openapi.json
  format: json
  label: aelf Node Web API
  slug: aelf-node-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aelf-inc/refs/heads/main/openapi/aelf-inc-node-web-api-openapi.json
- filename: aelf-inc-agent-gateway-openapi.yaml
  format: yaml
  label: aelf Agent Gateway API
  slug: aelf-agent-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aelf-inc/refs/heads/main/openapi/aelf-inc-agent-gateway-openapi.yaml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Aelf Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aelf declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Aelf
provider_slug: aelf-inc
scheme_count: 0
schemes: []
slug: aelf-inc-authentication
source_filename: aelf-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: >-\n  https://docs.aelf.com/tools/web-api/net-api/ (Basic authentication on the peer operations),\n  https://github.com/AElfProject/aelf-agent-gateway#readme (bearer + NyxID delegation JWT),\n  https://raw.githubusercontent.com/AElfProject/AElf/dev/src/AElf.WebApp.Application.Chain/Error.cs\n  and the two contracts in openapi/\nsummary: >-\n  The aelf node Web API is an unauthenticated API. There is no key, no token and no OAuth: reads\n  are open and even the transaction-submitting writes take no HTTP credential, because authority\n  travels inside the signed transaction rather than in a header. Two exceptions and one caveat:\n  the peer add/remove operations are documented as HTTP Basic, the self-hosted agent gateway uses\n  bearer plus a delegated JWT, and NEITHER of the node's auth requirements is declared in its\n  OpenAPI.\nsurfaces:\n- surface: aelf Node Web API\n  spec: openapi/aelf-inc-node-web-api-openapi.json\n \
  \ declared_security_schemes: []\n  effective_model: none (anonymous) for all /api/blockChain operations\n  authority_model: >-\n    Write authority is cryptographic, not HTTP. A transaction carries From, To, MethodName, Params,\n    RefBlockNumber/RefBlockPrefix and a Signature produced by the sender's private key; the node\n    validates the signature (error 20013 InvalidSignature) and the chain enforces permissions.\n    Sending a transaction is therefore an open endpoint that only accepts already-authorized bytes.\n  key_management: >-\n    Keys live client-side — created by `aelf-command create`, loaded from private key or mnemonic,\n    or held by a wallet (NightElf, Portkey). The API never sees them.\n  exceptions:\n  - operations:\n    - POST /api/net/peer\n    - DELETE /api/net/peer\n    scheme: http basic\n    documented_at: https://docs.aelf.com/tools/web-api/net-api/\n    source_signal: >-\n      Error.cs carries the constant NeedBasicAuth = \"User name and password for basic\
  \ auth should\n      be set\", confirming the node enforces it when configured.\n    gap: >-\n      The served OpenAPI declares NO securitySchemes at all, so these two operations look\n      anonymous to any machine reading the contract. A generated client will fail on them.\n- surface: aelf Agent Gateway\n  spec: openapi/aelf-inc-agent-gateway-openapi.yaml\n  declared_security_schemes:\n  - name: GatewayBearerAuth\n    type: http\n    scheme: bearer\n  effective_model: bearer token, plus NyxID identity and delegation JWTs in production\n  details:\n    open_operations:\n    - GET /health\n    - /openapi.json\n    - /docs\n    production_verification: signature, issuer, audience, scope and expiry\n    configuration:\n    - NYXID_JWKS_URL\n    - NYXID_ISSUER\n    - NYXID_AUDIENCE\n    - NYXID_REQUIRED_DELEGATION_SCOPE\n    admin_model: >-\n      Admin access derives only from a verified `sub` present in GATEWAY_ADMIN_NYX_USER_IDS;\n      role/scope headers cannot grant it. `trusted_headers`\
  \ identity is restricted to\n      non-production loopback development.\n    scopes_note: >-\n      A dedicated `wallet:write` delegation scope is named in the provider's own release notes as a\n      remaining blocker rather than a shipped feature, so no scope reference page exists and no\n      scopes/ artifact is emitted.\n- surface: MCP (aelf-node-skill)\n  transport: stdio\n  effective_model: none for reads; AELF_PRIVATE_KEY environment variable for writes\n  detail: mcp/aelf-inc-mcp.yml\noauth2: false\noidc: false\nmtls: false\napi_keys: false\ndiscovery_documents:\n  openid_configuration: absent\n  oauth_authorization_server: absent\n  probed: well-known/aelf-inc-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aelf-inc/refs/heads/main/authentication/aelf-inc-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Blockchain
- Layer 1
- Web3
- Smart Contracts
- Cross-Chain
- Developer Tools
- Protobuf
- Agent Skills
- Cryptocurrency
---
