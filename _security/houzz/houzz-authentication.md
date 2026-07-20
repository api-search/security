---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Houzz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Houzz secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Houzz
provider_slug: houzz
scheme_count: 1
schemes:
- credentials:
  - App ID
  - Token
  - User Name
  description: 'Static per-account credential set issued in the Houzz seller/vendor dashboard. Integrations present three values collected from Settings > API: App ID (application identifier), Token (secret access token), and User Name (account identifier). Sent by the integrating platform to authenticate catalog, inventory, pricing, and order calls.'
  name: HouzzAppCredentials
  scheme: token
  sources:
  - https://help.houzz.com/s/topic/0TO44000000UgcMGAS/houzz-seller-api?language=en_US
  type: apiKey
slug: houzz-authentication
source_filename: houzz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://help.houzz.com/s/topic/0TO44000000UgcMGAS/houzz-seller-api?language=en_US\ndocs: https://help.houzz.com/s/topic/0TO44000000UgcMGAS/houzz-seller-api?language=en_US\napi: Houzz Seller & Vendor Commerce API\nnotes: >-\n  Derived from Houzz seller/vendor API documentation and consistent third-party\n  integration guides (Sellercloud, Extensiv, CommerceBear). No first-party\n  OpenAPI is published, so scheme names below are descriptive of the documented\n  credential model, not machine-read from a spec. Access is partner-gated:\n  enable under Settings > API in the Houzz dashboard, or request via\n  sellerapi@houzz.com. Houzz Vendor and Houzz Seller are distinct programs and\n  a given integration must select the correct one.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  gated: true\n  access_request: sellerapi@houzz.com\nschemes:\n- name: HouzzAppCredentials\n  type: apiKey\n  scheme:\
  \ token\n  description: >-\n    Static per-account credential set issued in the Houzz seller/vendor\n    dashboard. Integrations present three values collected from Settings > API:\n    App ID (application identifier), Token (secret access token), and User Name\n    (account identifier). Sent by the integrating platform to authenticate\n    catalog, inventory, pricing, and order calls.\n  credentials:\n  - App ID\n  - Token\n  - User Name\n  sources:\n  - https://help.houzz.com/s/topic/0TO44000000UgcMGAS/houzz-seller-api?language=en_US\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/houzz/refs/heads/main/authentication/houzz-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ecommerce
- Marketplace
- Home Improvement
- Interior Design
- Home Renovation
- Furniture
- SaaS
---
