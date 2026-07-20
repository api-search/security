---
api_key_in:
- header
api_specs:
- filename: b3-b3os-workflow-openapi.json
  format: json
  label: B3OS Workflow API
  slug: b3os-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3/refs/heads/main/openapi/b3-b3os-workflow-openapi.json
auth_types:
- apiKey
- custom
description: ''
kind: authentication
layout: security
method: searched
name: B3 Authentication
name_suffix: Authentication
oauth_flows: []
overview: B3 secures its APIs with apiKey and custom across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: B3
provider_slug: b3
scheme_count: 0
schemes: []
slug: b3-authentication
source_filename: b3-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.b3.fun/sdk/global-account/authentication\ndocs: https://docs.b3.fun/sdk/api-key-request\nnote: >-\n  The B3OS Workflow OpenAPI declares no securitySchemes, so the mechanical\n  derive produced nothing; this profile is captured from the B3 developer docs.\n  B3 exposes three distinct authentication surfaces across its products.\nsummary:\n  types: [apiKey, custom]\n  api_key_in: [header]\nsurfaces:\n  - name: B3OS Workflow API\n    api: openapi/b3-b3os-workflow-openapi.json\n    scheme: api-key\n    detail: >-\n      API-key auth. The API exposes an api-keys resource (create/list/revoke) and\n      per-organization webhook secrets. Request a key via docs.b3.fun/sdk/api-key-request.\n    docs: https://docs.b3.fun/sdk/api-key-request\n  - name: B3 Data API\n    scheme: none\n    detail: >-\n      Public, no authentication required. Blockscout + Thirdweb Insights indexed\n      data is served free with no key for public\
  \ endpoints.\n    docs: https://docs.b3.fun/data/api-reference/introduction\n  - name: B3 Global Accounts (SDK)\n    scheme: global-accounts\n    detail: >-\n      End-user authentication via B3 Global Accounts — social login (Google,\n      Discord), headless auth service, session keys and scoped permissions.\n      Consumed client-side through @b3dotfun/sdk (useB3 / useAccountWallet hooks).\n    docs: https://docs.b3.fun/sdk/global-account/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/b3/refs/heads/main/authentication/b3-authentication.yml
summary_line: apiKey/custom · 0 schemes
tags:
- Company
- Crypto
- Blockchain
- Web3
- Workflow Automation
- Onchain Data
- Gaming
- Payments
- Layer 3
- Developer Tools
---
