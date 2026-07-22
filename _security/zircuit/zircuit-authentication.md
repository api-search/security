---
api_key_in: []
api_specs:
- filename: zircuit-gud-trading-engine-openapi.yml
  format: yaml
  label: Zircuit GUD Trading Engine API (Beta)
  slug: zircuit-gud-trading-engine-api-beta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zircuit/refs/heads/main/openapi/zircuit-gud-trading-engine-openapi.yml
auth_types:
- http
- none
description: ''
kind: authentication
layout: security
method: searched
name: Zircuit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zircuit secures its APIs with http and none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Zircuit
provider_slug: zircuit
scheme_count: 2
schemes:
- api: Zircuit GUD Trading Engine API (Beta)
  description: 'API key passed as an HTTP Bearer token (Authorization: Bearer <API_KEY>). Keys are provisioned by the Zircuit team and are also shared at hackathons; contact the team to obtain one.'
  docs: https://docs.zircuit.com/infra/gud-trading-engine-beta/api-endpoint
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zircuit-gud-trading-engine-openapi.yml
  type: http
- api: Zircuit JSON-RPC API
  description: Public, unauthenticated Ethereum JSON-RPC 2.0 access over HTTPS and WSS. No API key required for the community endpoints; paid dedicated node access is offered by DRPC.
  docs: https://docs.zircuit.com/infra/rpcs
  name: publicRpc
  type: none
slug: zircuit-authentication
source_filename: zircuit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/zircuit-gud-trading-engine-openapi.yml\ndocs: https://docs.zircuit.com/infra/gud-trading-engine-beta/api-endpoint\nsummary:\n  types:\n  - http\n  - none\n  notes: >-\n    Zircuit exposes two distinct API surfaces with different auth models. The\n    public Ethereum JSON-RPC endpoints (mainnet.zircuit.com,\n    garfield-testnet.zircuit.com) are unauthenticated public RPC — access is\n    open, with paid higher-throughput node access available from third parties\n    such as DRPC. The GUD Trading Engine REST API requires an HTTP Bearer API\n    key provisioned by the Zircuit team.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  api: Zircuit GUD Trading Engine API (Beta)\n  description: >-\n    API key passed as an HTTP Bearer token (Authorization: Bearer <API_KEY>).\n    Keys are provisioned by the Zircuit team and are also shared at hackathons;\n    contact the team to obtain one.\n  docs: https://docs.zircuit.com/infra/gud-trading-engine-beta/api-endpoint\n\
  \  sources:\n  - openapi/zircuit-gud-trading-engine-openapi.yml\n- name: publicRpc\n  type: none\n  api: Zircuit JSON-RPC API\n  description: >-\n    Public, unauthenticated Ethereum JSON-RPC 2.0 access over HTTPS and WSS.\n    No API key required for the community endpoints; paid dedicated node access\n    is offered by DRPC.\n  docs: https://docs.zircuit.com/infra/rpcs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zircuit/refs/heads/main/authentication/zircuit-authentication.yml
summary_line: http/none · 2 schemes
tags:
- Company
- Crypto
- Blockchain
- Layer 2
- Rollup
- Zero Knowledge
- EVM
- DeFi
- JSON-RPC
- Web3
---
