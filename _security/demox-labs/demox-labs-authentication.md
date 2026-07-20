---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Demox Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Demox Labs secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Demox Labs
provider_slug: demox-labs
scheme_count: 1
schemes:
- description: No authentication required; open JSON-RPC 2.0 endpoint, subject to rate limiting.
  name: public
  sources:
  - https://docs.leo.app/aleo-rpc-api
  type: none
slug: demox-labs-authentication
source_filename: demox-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.leo.app/aleo-rpc-api\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The public Aleo RPC API is free and requires no authentication — no API key,\n    token, or OAuth flow. The documentation notes that rate limiting may be\n    introduced to prevent spamming. Access is open over HTTPS against the\n    per-network JSON-RPC base URLs.\nschemes:\n- name: public\n  type: none\n  description: No authentication required; open JSON-RPC 2.0 endpoint, subject to\n    rate limiting.\n  sources: [https://docs.leo.app/aleo-rpc-api]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demox-labs/refs/heads/main/authentication/demox-labs-authentication.yml
summary_line: none · 1 scheme
tags:
- Company
- Blockchain
- Zero Knowledge
- Cryptocurrency
- Wallet
- Privacy
- Web3
- Developer Tools
- SDK
- JSON-RPC
---
