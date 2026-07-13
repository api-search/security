---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: BTCPay Server Greenfield API
  slug: btcpay-server-greenfield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcpay/refs/heads/main/openapi/openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Btcpay Authentication
name_suffix: Authentication
oauth_flows: []
overview: BTCPay Server secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BTCPay Server
provider_slug: btcpay
scheme_count: 2
schemes:
- description: 'BTCPay Server API key. Format: ''token {apiKey}'''
  in: header
  name: API_Key
  parameter: Authorization
  sources:
  - openapi/openapi.json
  type: apiKey
- description: HTTP Basic Authentication with email and password
  name: Basic
  scheme: basic
  sources:
  - openapi/openapi.json
  type: http
slug: btcpay-authentication
source_filename: btcpay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: API_Key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'BTCPay Server API key. Format: ''token {apiKey}'''\n  sources:\n  - openapi/openapi.json\n- name: Basic\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication with email and password\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/btcpay/refs/heads/main/authentication/btcpay-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Bitcoin
- Cryptocurrency
- Payments
- Lightning Network
- Open Source
- Self-Hosted
---
