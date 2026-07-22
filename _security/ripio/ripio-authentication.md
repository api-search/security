---
api_key_in: []
api_specs:
- filename: ripio-trade-openapi.yml
  format: yaml
  label: Ripio Trade API v4
  slug: ripio-trade-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripio/refs/heads/main/openapi/ripio-trade-openapi.yml
auth_types:
- apiToken
description: ''
kind: authentication
layout: security
method: derived
name: Ripio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ripio secures its APIs with apiToken across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ripio
provider_slug: ripio
scheme_count: 1
schemes:
- description: "You can create API Credentials on: <https://trade.ripio.com/market/api/token>.\n\n After creating the **API Credentials**, you'll need to save in a safe place two pieces of information, an **API Token** and a **Secret Key**. The credentials are required respectively to **Authenticate** and **Sign** all Private REST Requests.\n\n **Attention**: The Secret Key can only be viewed once and cannot be retri"
  name: API Credentials
  sources:
  - openapi/ripio-trade-openapi.yml
  type: apiToken
slug: ripio-authentication
source_filename: ripio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/ripio-trade-openapi.yml\nsummary:\n  types:\n  - apiToken\nschemes:\n- name: API Credentials\n  type: apiToken\n  description: |-\n    You can create API Credentials on: <https://trade.ripio.com/market/api/token>.\n\n     After creating the **API Credentials**, you'll need to save in a safe place two pieces of information, an **API Token** and a **Secret Key**. The credentials are required respectively to **Authenticate** and **Sign** all Private REST Requests.\n\n     **Attention**: The Secret Key can only be viewed once and cannot be retri\n  sources:\n  - openapi/ripio-trade-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ripio/refs/heads/main/authentication/ripio-authentication.yml
summary_line: apiToken · 1 scheme
tags:
- Company
- Crypto
- Cryptocurrency
- Exchange
- Trading
- Blockchain
- Latin America
- Bitcoin
- Stablecoins
- API
---
