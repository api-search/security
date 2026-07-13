---
api_key_in:
- header
api_specs:
- filename: celcoin-billissuance-settlement-openapi.json
  format: json
  label: Celcoin BaaS and Core Banking API
  slug: baas-core-banking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-billissuance-settlement-openapi.json
- filename: celcoin-credit-openapi.json
  format: json
  label: Celcoin Credit as a Service API
  slug: credit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-credit-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Celcoin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Celcoin secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Celcoin
provider_slug: celcoin
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: Autenticação utilizando JTW Bearer Token
  name: Bearer
  scheme: Bearer
  sources:
  - openapi/celcoin-billissuance-settlement-openapi.json
  type: http
- bearerFormat: JWT
  description: 'JWT Authorization header using the Bearer scheme. Example: "Authorization: Bearer {token}"'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/celcoin-credit-openapi.json
  type: http
- description: '[API V5] - Please enter into field the word ''Bearer'' following by space and the access_token (JWT)'
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/celcoin-onboarding-openapi.json
  type: apiKey
slug: celcoin-authentication
source_filename: celcoin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/celcoin-billissuance-settlement-openapi.json, openapi/celcoin-credit-openapi.json,\n  openapi/celcoin-onboarding-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  description: Autenticação utilizando JTW Bearer Token\n  sources:\n  - openapi/celcoin-billissuance-settlement-openapi.json\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT Authorization header using the Bearer scheme. Example: \"Authorization: Bearer\n    {token}\"'\n  sources:\n  - openapi/celcoin-credit-openapi.json\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: '[API V5] - Please enter into field the word ''Bearer'' following by space and\n    the access_token (JWT)'\n  sources:\n  - openapi/celcoin-onboarding-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/authentication/celcoin-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Banking as a Service
- BaaS
- Pix
- Boleto
- TED
- Bill Payments
- Prepaid Cards
- Digital Accounts
- Open Banking
- Open Finance
- Credit
- Fintech
- Brazil
- Financial Infrastructure
---
