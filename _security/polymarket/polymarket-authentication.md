---
api_key_in:
- header
api_specs:
- filename: polymarket-asyncapi.yml
  format: yaml
  label: Polymarket WebSocket
  slug: websocket
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymarket/refs/heads/main/asyncapi/polymarket-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Polymarket Authentication
name_suffix: Authentication
oauth_flows: []
overview: Polymarket secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Polymarket
provider_slug: polymarket
scheme_count: 1
schemes:
- description: 'Polymarket CLOB authenticated trading endpoints require five

    headers: POLY_API_KEY, POLY_ADDRESS, POLY_SIGNATURE,

    POLY_PASSPHRASE, POLY_TIMESTAMP. Only POLY_API_KEY is modelled

    here because OpenAPI security schemes describe a single header

    each; in practice, all five must be sent on each request.'
  in: header
  name: polyApiSignature
  parameter: POLY_API_KEY
  sources:
  - openapi/polymarket-openapi.yml
  type: apiKey
slug: polymarket-authentication
source_filename: polymarket-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/polymarket-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: polyApiSignature\n  type: apiKey\n  in: header\n  parameter: POLY_API_KEY\n  description: |-\n    Polymarket CLOB authenticated trading endpoints require five\n    headers: POLY_API_KEY, POLY_ADDRESS, POLY_SIGNATURE,\n    POLY_PASSPHRASE, POLY_TIMESTAMP. Only POLY_API_KEY is modelled\n    here because OpenAPI security schemes describe a single header\n    each; in practice, all five must be sent on each request.\n  sources:\n  - openapi/polymarket-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polymarket/refs/heads/main/authentication/polymarket-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Prediction Markets
- DeFi
- Polygon
- Order Book
- Crypto
- Markets
---
