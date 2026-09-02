---
api_key_in:
- header
api_specs:
- filename: mystars-mystars-faas-fulfilment-api-api-openapi.yml
  format: yaml
  label: MyStars FaaS MyStars FaaS — Fulfilment API
  slug: mystars-mystars-faas-fulfilment-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystars/refs/heads/main/openapi/mystars-mystars-faas-fulfilment-api-api-openapi.yml
- filename: mystars-orders-api-openapi.yml
  format: yaml
  label: MyStars FaaS Orders API
  slug: mystars-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystars/refs/heads/main/openapi/mystars-orders-api-openapi.yml
- filename: mystars-pricing-api-openapi.yml
  format: yaml
  label: MyStars FaaS Pricing API
  slug: mystars-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystars/refs/heads/main/openapi/mystars-pricing-api-openapi.yml
- filename: mystars-recipients-api-openapi.yml
  format: yaml
  label: MyStars FaaS Recipients API
  slug: mystars-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mystars/refs/heads/main/openapi/mystars-recipients-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mystars Authentication
name_suffix: Authentication
oauth_flows: []
overview: MyStars FaaS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MyStars FaaS
provider_slug: mystars
scheme_count: 1
schemes:
- description: 'Your secret API key. Get one from [@my_stars_tg_bot](https://t.me/my_stars_tg_bot) → **API access**, then send it in the `X-Api-Key` header on every request. Treat it like a password — anyone with the key can create orders on your tenant, read your order history, and cancel unpaid orders. Each order is settled by its own on-chain payment, so the key by itself cannot move funds. Rotate it any time '
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/mystars-faas-openapi.json
  type: apiKey
slug: mystars-authentication
source_filename: mystars-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: derived\nsource: openapi/mystars-faas-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: 'Your secret API key. Get one from [@my_stars_tg_bot](https://t.me/my_stars_tg_bot)\n    → **API access**, then send it in the `X-Api-Key` header on every request. Treat it like\n    a password — anyone with the key can create orders on your tenant, read your order history,\n    and cancel unpaid orders. Each order is settled by its own on-chain payment, so the key\n    by itself cannot move funds. Rotate it any time '\n  sources:\n  - openapi/mystars-faas-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mystars/refs/heads/main/authentication/mystars-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Telegram
- telegram-stars
- telegram-premium
- Payments
- Crypto
- TON
- fulfilment
- Blockchain
- Digital Goods
- reseller-api
---
