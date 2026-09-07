---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: MyStars FaaS Fulfilment API
  slug: mystars-faas-fulfilment-api
  spec_type: OpenAPI
  url: https://mystars.tg/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Mystars Faas Fulfilment Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: MyStars FaaS — Fulfilment API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MyStars FaaS — Fulfilment API
provider_slug: mystars-faas-fulfilment-api
scheme_count: 1
schemes:
- description: 'Your secret API key. Get one from [@my_stars_tg_bot](https://t.me/my_stars_tg_bot) → **API access**, then send it in the `X-Api-Key` header on every request. Treat it like a password — anyone with the key can create orders on your tenant, read your order history, and cancel unpaid orders. Each order is settled by its own on-chain payment, so the key by itself cannot move funds. Rotate it any time '
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/mystars-faas-fulfilment-api-openapi-original.json
  type: apiKey
slug: mystars-faas-fulfilment-api-authentication
source_filename: mystars-faas-fulfilment-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: derived\nsource: openapi/mystars-faas-fulfilment-api-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: 'Your secret API key. Get one from [@my_stars_tg_bot](https://t.me/my_stars_tg_bot)\n    → **API access**, then send it in the `X-Api-Key` header on every request. Treat it like\n    a password — anyone with the key can create orders on your tenant, read your order history,\n    and cancel unpaid orders. Each order is settled by its own on-chain payment, so the key\n    by itself cannot move funds. Rotate it any time '\n  sources:\n  - openapi/mystars-faas-fulfilment-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mystars-faas-fulfilment-api/refs/heads/main/authentication/mystars-faas-fulfilment-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Telegram
- telegram-stars
- telegram-premium
- Payments
- Crypto
- TON
- gram
- USDT
- Fintech
- fulfilment
- Digital Goods
- Non-Custodial
- no-kyc
---
