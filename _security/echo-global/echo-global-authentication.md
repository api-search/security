---
api_key_in:
- header
api_specs:
- filename: echo-global-documents-api-openapi.yml
  format: yaml
  label: Echo Global Logistics documents API
  slug: echo-global-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/echo-global/refs/heads/main/openapi/echo-global-documents-api-openapi.yml
- filename: echo-global-health-api-openapi.yml
  format: yaml
  label: Echo Global Logistics health API
  slug: echo-global-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/echo-global/refs/heads/main/openapi/echo-global-health-api-openapi.yml
- filename: echo-global-ping-api-openapi.yml
  format: yaml
  label: Echo Global Logistics ping API
  slug: echo-global-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/echo-global/refs/heads/main/openapi/echo-global-ping-api-openapi.yml
- filename: echo-global-query-api-openapi.yml
  format: yaml
  label: Echo Global Logistics query API
  slug: echo-global-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/echo-global/refs/heads/main/openapi/echo-global-query-api-openapi.yml
- filename: echo-global-quotes-api-openapi.yml
  format: yaml
  label: Echo Global Logistics quotes API
  slug: echo-global-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/echo-global/refs/heads/main/openapi/echo-global-quotes-api-openapi.yml
- filename: echo-global-rates-api-openapi.yml
  format: yaml
  label: Echo Global Logistics rates API
  slug: echo-global-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/echo-global/refs/heads/main/openapi/echo-global-rates-api-openapi.yml
- filename: echo-global-shipments-api-openapi.yml
  format: yaml
  label: Echo Global Logistics shipments API
  slug: echo-global-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/echo-global/refs/heads/main/openapi/echo-global-shipments-api-openapi.yml
- filename: echo-global-token-api-openapi.yml
  format: yaml
  label: Echo Global Logistics token API
  slug: echo-global-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/echo-global/refs/heads/main/openapi/echo-global-token-api-openapi.yml
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
