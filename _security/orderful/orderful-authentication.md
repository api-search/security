---
api_key_in:
- header
api_specs:
- filename: orderful-openapi-original.yml
  format: yaml
  label: Orderful API (Mosaic / v3)
  slug: orderful-api-mosaic-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Orderful Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orderful secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orderful
provider_slug: orderful
scheme_count: 1
schemes:
- in: header
  name: API_KEY
  parameter: orderful-api-key
  sources:
  - openapi/orderful-openapi-original.yml
  type: apiKey
slug: orderful-authentication
source_filename: orderful-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/orderful-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: API_KEY\n  type: apiKey\n  in: header\n  parameter: orderful-api-key\n  sources:\n  - openapi/orderful-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/authentication/orderful-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- EDI
- Electronic Data Interchange
- Supply Chain
- B2B
- Logistics
- Retail
- Transactions
- Integration
---
