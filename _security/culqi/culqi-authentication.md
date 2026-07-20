---
api_key_in: []
api_specs:
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Tokens API
  slug: culqi-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Charges API
  slug: culqi-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Orders API
  slug: culqi-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Refunds API
  slug: culqi-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Customers API
  slug: culqi-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Cards API
  slug: culqi-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Plans API
  slug: culqi-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Subscriptions API
  slug: culqi-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Events & Webhooks API
  slug: culqi-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi IIN Lookup API
  slug: culqi-iin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Transfers API
  slug: culqi-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: modeled-from-docs
name: Culqi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Culqi secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Culqi
provider_slug: culqi
scheme_count: 2
schemes:
- bearerFormat: sk_live_/sk_test_ secret key
  host: https://api.culqi.com/v2
  name: secret_key
  scheme: bearer
  sources:
  - openapi/culqi-openapi.yml
  - https://docs.culqi.com/
  type: http
  usage: Server-side operations (charges, orders, refunds, customers, cards, plans, subscriptions, events, iins, transfers).
- bearerFormat: pk_live_/pk_test_ public key
  host: https://secure.culqi.com/v2
  name: public_key
  scheme: bearer
  sources:
  - openapi/culqi-openapi.yml
  - https://docs.culqi.com/
  type: http
  usage: Client-side card/Yape tokenization (POST /tokens, /tokens/yape) and 3DS charge confirmation (POST /confirm).
slug: culqi-authentication
source_filename: culqi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: modeled-from-docs\nsource: https://docs.culqi.com/ + openapi/culqi-openapi.yml\nsummary:\n  types:\n  - http\nnotes: >-\n  Culqi API v2 uses HTTP Bearer authentication with two key types. Card\n  tokenization and 3DS confirmation on the secure host (secure.culqi.com/v2)\n  use the public key (pk_live_/pk_test_). All server-side money-movement and\n  management operations on the API host (api.culqi.com/v2) use the secret key\n  (sk_live_/sk_test_) and must never be exposed client-side. Keys are issued\n  in the CulqiPanel under Development > API Keys.\nschemes:\n- name: secret_key\n  type: http\n  scheme: bearer\n  bearerFormat: sk_live_/sk_test_ secret key\n  host: https://api.culqi.com/v2\n  usage: Server-side operations (charges, orders, refunds, customers, cards, plans, subscriptions, events, iins, transfers).\n  sources:\n  - openapi/culqi-openapi.yml\n  - https://docs.culqi.com/\n- name: public_key\n  type: http\n  scheme: bearer\n  bearerFormat:\
  \ pk_live_/pk_test_ public key\n  host: https://secure.culqi.com/v2\n  usage: Client-side card/Yape tokenization (POST /tokens, /tokens/yape) and 3DS charge confirmation (POST /confirm).\n  sources:\n  - openapi/culqi-openapi.yml\n  - https://docs.culqi.com/\ncompliance:\n  pciDss: >-\n    Merchants interacting directly with the API (rather than Culqi Checkout /\n    Culqi JS v4 client-side tokenization) must comply with PCI DSS 3.2 and\n    submit an SAQ-D form to Culqi's risk team. Culqi recommends tokenizing\n    card data client-side so raw PAN never touches the merchant server.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/authentication/culqi-authentication.yml
summary_line: http · 2 schemes
tags:
- Payments
- Payment Gateway
- FinTech
- Peru
- LatAm
- Cards
- Yape
---
