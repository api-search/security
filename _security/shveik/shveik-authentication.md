---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: shveik-discovery-api-openapi.yml
  format: yaml
  label: shveik Discovery API
  slug: shveik-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shveik/refs/heads/main/openapi/shveik-discovery-api-openapi.yml
- filename: shveik-scraping-api-openapi.yml
  format: yaml
  label: shveik Scraping API
  slug: shveik-scraping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shveik/refs/heads/main/openapi/shveik-scraping-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Shveik Authentication
name_suffix: Authentication
oauth_flows: []
overview: shveik secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: shveik
provider_slug: shveik
scheme_count: 2
schemes:
- description: MPP evm/authorization credential in Authorization header. First request without payment returns WWW-Authenticate challenge.
  name: mpp
  scheme: Payment
  sources:
  - openapi/shveik-agdata-openapi.yml
  - openapi/shveik-agmail-openapi.yml
  - openapi/shveik-agpay-openapi.yml
  - openapi/shveik-agproxy-openapi.yml
  - openapi/shveik-agvps-openapi.yml
  type: http
- description: x402 exact payment credential. First request without payment returns PAYMENT-REQUIRED quote.
  in: header
  name: x402
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/shveik-agdata-openapi.yml
  - openapi/shveik-agmail-openapi.yml
  - openapi/shveik-agpay-openapi.yml
  - openapi/shveik-agproxy-openapi.yml
  - openapi/shveik-agvps-openapi.yml
  type: apiKey
slug: shveik-authentication
source_filename: shveik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: derived\nsource: openapi/shveik-agdata-openapi.yml, openapi/shveik-agmail-openapi.yml, openapi/shveik-agpay-openapi.yml,\n  openapi/shveik-agproxy-openapi.yml, openapi/shveik-agvps-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: mpp\n  type: http\n  scheme: Payment\n  description: MPP evm/authorization credential in Authorization header. First request without\n    payment returns WWW-Authenticate challenge.\n  sources:\n  - openapi/shveik-agdata-openapi.yml\n  - openapi/shveik-agmail-openapi.yml\n  - openapi/shveik-agpay-openapi.yml\n  - openapi/shveik-agproxy-openapi.yml\n  - openapi/shveik-agvps-openapi.yml\n- name: x402\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: x402 exact payment credential. First request without payment returns PAYMENT-REQUIRED\n    quote.\n  sources:\n  - openapi/shveik-agdata-openapi.yml\n  - openapi/shveik-agmail-openapi.yml\n  - openapi/shveik-agpay-openapi.yml\n\
  \  - openapi/shveik-agproxy-openapi.yml\n  - openapi/shveik-agvps-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shveik/refs/heads/main/authentication/shveik-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- AI Agents
- x402
- Web Scraping
- Proxies
- Email
- VPS
- Escrow
- MCP
- Stablecoins
---
