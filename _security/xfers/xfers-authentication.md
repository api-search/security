---
api_key_in:
- header
- query
api_specs:
- filename: xfers-singapore-openapi.json
  format: json
  label: Xfers Singapore API
  slug: xfers-singapore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xfers/refs/heads/main/openapi/xfers-singapore-openapi.json
- filename: xfers-indonesia-openapi.json
  format: json
  label: Xfers Indonesia API
  slug: xfers-indonesia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xfers/refs/heads/main/openapi/xfers-indonesia-openapi.json
- filename: xfers-indonesia-payment-gateway-unique-amount-openapi.json
  format: json
  label: Xfers Indonesia Payment Gateway API
  slug: xfers-indonesia-payment-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xfers/refs/heads/main/openapi/xfers-indonesia-payment-gateway-unique-amount-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Xfers Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xfers secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Xfers
provider_slug: xfers
scheme_count: 4
schemes:
- description: You can retrieve this from your merchant's dashboard
  in: header
  name: X-XFERS-APP-API-KEY
  parameter: X-XFERS-APP-API-KEY
  sources:
  - openapi/xfers-indonesia-openapi.json
  - openapi/xfers-indonesia-payment-gateway-unique-amount-openapi.json
  - openapi/xfers-indonesia-payment-gateway-va-cvs-openapi.json
  - openapi/xfers-singapore-openapi.json
  type: apiKey
- description: You can retrieve this by using [get_token API](../sg/api/cutting-edge#operation/getToken)
  in: header
  name: X-XFERS-USER-API-KEY
  parameter: X-XFERS-USER-API-KEY
  sources:
  - openapi/xfers-indonesia-openapi.json
  - openapi/xfers-indonesia-payment-gateway-unique-amount-openapi.json
  - openapi/xfers-indonesia-payment-gateway-va-cvs-openapi.json
  - openapi/xfers-singapore-openapi.json
  type: apiKey
- description: You can retrieve this by using [get_token API](../sg/api/cutting-edge#operation/getToken)
  in: query
  name: user-api-token
  parameter: X-XFERS-USER-API-KEY
  sources:
  - openapi/xfers-indonesia-openapi.json
  - openapi/xfers-indonesia-payment-gateway-unique-amount-openapi.json
  - openapi/xfers-indonesia-payment-gateway-va-cvs-openapi.json
  - openapi/xfers-singapore-openapi.json
  type: apiKey
- bearerFormat: xfers_api_token
  description: "You can retrieve this from the dashboard. For instance: \n\n```\n\nAuthorization: Bearer <xfers_api_token>\n\n```"
  name: v4XfersAuth
  scheme: bearer
  sources:
  - openapi/xfers-indonesia-openapi.json
  - openapi/xfers-indonesia-payment-gateway-unique-amount-openapi.json
  - openapi/xfers-indonesia-payment-gateway-va-cvs-openapi.json
  - openapi/xfers-singapore-openapi.json
  type: http
slug: xfers-authentication
source_filename: xfers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/xfers-indonesia-openapi.json, openapi/xfers-indonesia-payment-gateway-unique-amount-openapi.json,\n  openapi/xfers-indonesia-payment-gateway-va-cvs-openapi.json, openapi/xfers-singapore-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: X-XFERS-APP-API-KEY\n  type: apiKey\n  in: header\n  parameter: X-XFERS-APP-API-KEY\n  description: You can retrieve this from your merchant's dashboard\n  sources:\n  - openapi/xfers-indonesia-openapi.json\n  - openapi/xfers-indonesia-payment-gateway-unique-amount-openapi.json\n  - openapi/xfers-indonesia-payment-gateway-va-cvs-openapi.json\n  - openapi/xfers-singapore-openapi.json\n- name: X-XFERS-USER-API-KEY\n  type: apiKey\n  in: header\n  parameter: X-XFERS-USER-API-KEY\n  description: You can retrieve this by using [get_token API](../sg/api/cutting-edge#operation/getToken)\n  sources:\n  - openapi/xfers-indonesia-openapi.json\n\
  \  - openapi/xfers-indonesia-payment-gateway-unique-amount-openapi.json\n  - openapi/xfers-indonesia-payment-gateway-va-cvs-openapi.json\n  - openapi/xfers-singapore-openapi.json\n- name: user-api-token\n  type: apiKey\n  in: query\n  parameter: X-XFERS-USER-API-KEY\n  description: You can retrieve this by using [get_token API](../sg/api/cutting-edge#operation/getToken)\n  sources:\n  - openapi/xfers-indonesia-openapi.json\n  - openapi/xfers-indonesia-payment-gateway-unique-amount-openapi.json\n  - openapi/xfers-indonesia-payment-gateway-va-cvs-openapi.json\n  - openapi/xfers-singapore-openapi.json\n- name: v4XfersAuth\n  type: http\n  scheme: bearer\n  bearerFormat: xfers_api_token\n  description: \"You can retrieve this from the dashboard. For instance: \\n\\n```\\n\\nAuthorization:\\\n    \\ Bearer <xfers_api_token>\\n\\n```\"\n  sources:\n  - openapi/xfers-indonesia-openapi.json\n  - openapi/xfers-indonesia-payment-gateway-unique-amount-openapi.json\n  - openapi/xfers-indonesia-payment-gateway-va-cvs-openapi.json\n\
  \  - openapi/xfers-singapore-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xfers/refs/heads/main/authentication/xfers-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Payments
- Fintech
- Bank Transfers
- Digital Wallets
- Lending
- Singapore
- Indonesia
- Southeast Asia
---
