---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: EchoSync Partner-Connect API
  slug: echosync-partner-connect-api
  spec_type: OpenAPI
  url: https://app.swaggerhub.com/apis/echogl/rest-api/
- filename: openapi.yaml
  format: yaml
  label: EchoSync Customer API
  slug: echosync-customer-api
  spec_type: OpenAPI
  url: https://app.swaggerhub.com/apis-docs/echogl/Customer_API_OAuth_Public/
- filename: openapi.yaml
  format: yaml
  label: EchoSync Carrier API
  slug: echosync-carrier-api
  spec_type: OpenAPI
  url: https://app.swaggerhub.com/apis-docs/echogl/Carrier_API_Public/
- filename: openapi.yaml
  format: yaml
  label: EchoSync Authorizer API
  slug: echosync-authorizer-api
  spec_type: OpenAPI
  url: https://app.swaggerhub.com/apis-docs/echogl/Echo_Authorizer_Public/
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Echo Global Authentication
name_suffix: Authentication
oauth_flows: []
overview: Echo Global Logistics secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Echo Global Logistics
provider_slug: echo-global
scheme_count: 3
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/echosync-authorizer-api.json
  - openapi/echosync-partner-connect-api.json
  type: http
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/echosync-authorizer-api.json
  type: apiKey
- in: header
  name: customer_api_authorizer_post
  parameter: Authorization
  sources:
  - openapi/echosync-customer-api.json
  type: apiKey
slug: echo-global-authentication
source_filename: echo-global-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/echosync-authorizer-api.json, openapi/echosync-customer-api.json, openapi/echosync-partner-connect-api.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/echosync-authorizer-api.json\n  - openapi/echosync-partner-connect-api.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/echosync-authorizer-api.json\n- name: customer_api_authorizer_post\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/echosync-customer-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echo-global/refs/heads/main/authentication/echo-global-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Freight
- Logistics
- Shipping
- LTL
- Truckload
- Freight Brokerage
- Transportation
- Supply Chain
---
