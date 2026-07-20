---
api_key_in:
- header
api_specs:
- filename: idrx-openapi.yml
  format: yaml
  label: IDRX API
  slug: idrx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idrx/refs/heads/main/openapi/idrx-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Idrx Authentication
name_suffix: Authentication
oauth_flows: []
overview: IDRX secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IDRX
provider_slug: idrx
scheme_count: 1
schemes:
- description: API key issued by IDRX. Each request must also carry `idrx-api-sig` (an HMAC-SHA256 signature) and `idrx-api-ts` (Unix ms timestamp), plus a custom `User-Agent`. Signature = HMAC-SHA256(secret, METHOD + ":" + PATH + ":" + SHA256(body) + ":" + timestamp).
  in: header
  name: idrxApiKey
  parameter: idrx-api-key
  sources:
  - openapi/idrx-openapi.yml
  type: apiKey
slug: idrx-authentication
source_filename: idrx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/idrx-openapi.yml\ndocs: https://docs.idrx.co/api/generating-a-signature\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: idrxApiKey\n  type: apiKey\n  in: header\n  parameter: idrx-api-key\n  description: API key issued by IDRX. Each request must also carry `idrx-api-sig` (an HMAC-SHA256\n    signature) and `idrx-api-ts` (Unix ms timestamp), plus a custom `User-Agent`. Signature\n    = HMAC-SHA256(secret, METHOD + \":\" + PATH + \":\" + SHA256(body) + \":\" + timestamp).\n  sources:\n  - openapi/idrx-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idrx/refs/heads/main/authentication/idrx-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Stablecoin
- Cryptocurrency
- Payments
- Blockchain
- Fintech
- Indonesia
- Rupiah
- Web3
- On-Ramp
- Digital Currency
---
