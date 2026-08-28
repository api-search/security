---
api_key_in:
- header
api_specs:
- filename: biconomy-instructions-api-openapi.yml
  format: yaml
  label: Biconomy instructions API
  slug: biconomy-instructions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biconomy/refs/heads/main/openapi/biconomy-instructions-api-openapi.yml
- filename: biconomy-mee-api-openapi.yml
  format: yaml
  label: Biconomy mee API
  slug: biconomy-mee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biconomy/refs/heads/main/openapi/biconomy-mee-api-openapi.yml
- filename: biconomy-root-api-openapi.yml
  format: yaml
  label: Biconomy root API
  slug: biconomy-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biconomy/refs/heads/main/openapi/biconomy-root-api-openapi.yml
auth_types:
- apiKey
- http-bearer
description: One credential, two hosts, two conventions. The project API key issued from the Biconomy Dashboard is sent as X-API-Key to api.biconomy.io and as an Authorization Bearer token to network.biconomy.io. There is no OAuth, no OIDC, no delegated identity and no scope system at the HTTP layer — authorization of what an agent may actually DO is pushed down to the on-chain Smart Sessions policy module, not expressed in the API credential.
kind: authentication
layout: security
method: searched
name: Biconomy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Biconomy secures its APIs with apiKey and http-bearer across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Biconomy
provider_slug: biconomy
scheme_count: 3
schemes:
- description: Project-scoped API key required by every Supertransaction API operation. Issued from https://dashboard.biconomy.io. Published example prefix is `mee_`.
  host: https://api.biconomy.io
  in: header
  issuance_url: https://dashboard.biconomy.io
  key_prefix: mee_
  name: X-API-Key
  parameter: X-API-Key
  rotation_policy: not published
  sources:
  - openapi/biconomy-root-api-openapi.yml
  - openapi/biconomy-mee-api-openapi.yml
  - openapi/biconomy-instructions-api-openapi.yml
  - https://docs.biconomy.io/supertransaction-api/openapi.yaml
  test_key_separation: false
  type: apiKey
- description: 'The MEE explorer/status surface takes the same dashboard-issued key as a Bearer token. Documented in https://docs.biconomy.io/llms.txt as "GET network.biconomy.io/v1/explorer/{hash}, Authorization: Bearer YOUR_API_KEY".'
  evidence:
    body: '{"errors":["API key required. Please visit https://dashboard.biconomy.io or join Biconomy Builders T..."]}'
    http_status: 401
    url: https://network.biconomy.io/v1/explorer/0x0
  host: https://network.biconomy.io
  in: header
  method: probed
  name: Authorization Bearer
  probed: '2026-08-24'
  scheme: bearer
  sources:
  - https://docs.biconomy.io/llms.txt
  - https://docs.biconomy.io/overview/supertransaction-api/execute
  type: http
- description: The Dashboard Public API (GET /api/public/projects/me/supertransactions) takes the same project key in a lowercase x-api-key header, per the worked example at https://docs.biconomy.io/overview/supertransaction-api/history-and-costs. HTTP header names are case-insensitive so this is not a functional difference, but it is a third documented spelling of the same credential and worth recording as such.
  host: https://dashboard.biconomy.io
  in: header
  name: x-api-key (lowercase)
  parameter: x-api-key
  sources:
  - https://docs.biconomy.io/overview/supertransaction-api/history-and-costs
  type: apiKey
slug: biconomy-authentication
source_filename: biconomy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-24'\nmethod: searched\nsource: >-\n  Derived from the securitySchemes in openapi/biconomy-root-api-openapi.yml (and the live specs at\n  https://docs.biconomy.io/supertransaction-api/openapi.yaml and\n  https://www.biconomy.io/openapi.json), then upgraded from the published docs at\n  https://docs.biconomy.io/overview/supertransaction-api and a live unauthenticated probe of\n  https://network.biconomy.io/v1/explorer/{hash} on 2026-08-24.\ndocs: https://docs.biconomy.io/overview/supertransaction-api\nprovider: Biconomy\nproviderId: biconomy\ndescription: >-\n  One credential, two hosts, two conventions. The project API key issued from the Biconomy\n  Dashboard is sent as X-API-Key to api.biconomy.io and as an Authorization Bearer token to\n  network.biconomy.io. There is no OAuth, no OIDC, no delegated identity and no scope system at\n  the HTTP layer — authorization of what an agent may actually DO is pushed down to the on-chain\n  Smart Sessions policy\
  \ module, not expressed in the API credential.\nsummary:\n  types:\n    - apiKey\n    - http-bearer\n  api_key_in:\n    - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: none\nschemes:\n  - name: X-API-Key\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n    host: https://api.biconomy.io\n    description: >-\n      Project-scoped API key required by every Supertransaction API operation. Issued from\n      https://dashboard.biconomy.io. Published example prefix is `mee_`.\n    issuance_url: https://dashboard.biconomy.io\n    key_prefix: mee_\n    rotation_policy: not published\n    test_key_separation: false\n    sources:\n      - openapi/biconomy-root-api-openapi.yml\n      - openapi/biconomy-mee-api-openapi.yml\n      - openapi/biconomy-instructions-api-openapi.yml\n      - https://docs.biconomy.io/supertransaction-api/openapi.yaml\n  - name: Authorization Bearer\n    type: http\n    scheme: bearer\n    in: header\n    host: https://network.biconomy.io\n\
  \    description: >-\n      The MEE explorer/status surface takes the same dashboard-issued key as a Bearer token.\n      Documented in https://docs.biconomy.io/llms.txt as\n      \"GET network.biconomy.io/v1/explorer/{hash}, Authorization: Bearer YOUR_API_KEY\".\n    method: probed\n    probed: '2026-08-24'\n    evidence:\n      url: https://network.biconomy.io/v1/explorer/0x0\n      http_status: 401\n      body: >-\n        {\"errors\":[\"API key required. Please visit https://dashboard.biconomy.io or join Biconomy\n        Builders T...\"]}\n    sources:\n      - https://docs.biconomy.io/llms.txt\n      - https://docs.biconomy.io/overview/supertransaction-api/execute\n  - name: x-api-key (lowercase)\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    host: https://dashboard.biconomy.io\n    description: >-\n      The Dashboard Public API (GET /api/public/projects/me/supertransactions) takes the same\n      project key in a lowercase x-api-key header, per the worked example\
  \ at\n      https://docs.biconomy.io/overview/supertransaction-api/history-and-costs. HTTP header names\n      are case-insensitive so this is not a functional difference, but it is a third documented\n      spelling of the same credential and worth recording as such.\n    sources:\n      - https://docs.biconomy.io/overview/supertransaction-api/history-and-costs\ndelegated_authorization:\n  http_layer: none\n  onchain_layer: Smart Sessions\n  detail: >-\n    Biconomy's answer to delegation is not an OAuth scope — it is an on-chain session grant. A user\n    grants a session key a set of policies (Sudo, Universal Action with parameter-level spending\n    caps, Time Range, Usage Limit) enforced by the ERC-7579 session module. The consequence is\n    real and cuts both ways: the permission boundary is stronger than a bearer scope because it is\n    enforced by contract rather than by the API, but it is invisible to any HTTP-layer tooling —\n    an API gateway, an MCP client or an agent framework\
  \ inspecting the credential learns nothing\n    about what the holder may do.\n  docs: https://docs.biconomy.io/agents-automation/policies\ndiscovery:\n  oauth_authorization_server: 404\n  oauth_protected_resource: 404\n  openid_configuration: 404\n  probed: '2026-08-24'\n  note: >-\n    All three probed on api.biconomy.io and docs.biconomy.io. No authorization-server metadata\n    exists, so an MCP client cannot bind a user to a Biconomy project through a standard flow.\ngaps:\n  - >-\n    No key rotation, expiry or revocation procedure is published, and no scope or permission model\n    attaches to the key — an API key is all-or-nothing against the project.\n  - >-\n    No separate test credential. A key cannot be inspected to tell whether it points at test or\n    live; separation is by chain ID and base URL only.\n  - >-\n    The same secret is presented under two different header conventions on two hosts, which is a\n    small but real source of integration error.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biconomy/refs/heads/main/authentication/biconomy-authentication.yml
summary_line: apiKey/http-bearer · 3 schemes
tags:
- Account Abstraction
- Blockchain
- Bundler
- Cross-Chain
- DeFi
- ERC-4337
- ERC-7579
- ERC-7702
- Ethereum
- Gas Abstraction
- Gasless
- MEE
- Paymaster
- Smart Accounts
- Smart Sessions
- Wallets
- Web3
---
