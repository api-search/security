---
api_key_in:
- header
api_specs:
- filename: fiserv-commercehub-openapi.yml
  format: yaml
  label: Fiserv CommerceHub API
  slug: commercehub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiserv/refs/heads/main/openapi/fiserv-commercehub-openapi.yml
- filename: fiserv-cardpointe-gateway-openapi.yml
  format: yaml
  label: Fiserv CardPointe Gateway API
  slug: cardpointe-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiserv/refs/heads/main/openapi/fiserv-cardpointe-gateway-openapi.yml
- filename: fiserv-bankinghub-openapi.yml
  format: yaml
  label: Fiserv BankingHub API
  slug: bankinghub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiserv/refs/heads/main/openapi/fiserv-bankinghub-openapi.yml
- filename: fiserv-carddeveloper-openapi.yml
  format: yaml
  label: Fiserv CardDeveloper API
  slug: carddeveloper
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiserv/refs/heads/main/openapi/fiserv-carddeveloper-openapi.yml
- filename: fiserv-payment-events-asyncapi.yml
  format: yaml
  label: Fiserv Payment Events
  slug: payment-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiserv/refs/heads/main/asyncapi/fiserv-payment-events-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fiserv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fiserv secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fiserv
provider_slug: fiserv
scheme_count: 4
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token for API authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fiserv-bankinghub-openapi.yml
  - openapi/fiserv-carddeveloper-openapi.yml
  type: http
- description: HTTP Basic authentication using the CardPointe Gateway credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/fiserv-cardpointe-gateway-openapi.yml
  type: http
- description: API key provided by Fiserv for authenticating requests.
  in: header
  name: apiKeyAuth
  parameter: Api-Key
  sources:
  - openapi/fiserv-commercehub-openapi.yml
  type: apiKey
- description: HMAC signature generated using the API secret, request timestamp, and request payload for message integrity verification.
  in: header
  name: hmacAuth
  parameter: Authorization
  sources:
  - openapi/fiserv-commercehub-openapi.yml
  type: apiKey
slug: fiserv-authentication
source_filename: fiserv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fiserv-bankinghub-openapi.yml, openapi/fiserv-carddeveloper-openapi.yml, openapi/fiserv-cardpointe-gateway-openapi.yml,\n  openapi/fiserv-commercehub-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token for API authentication.\n  sources:\n  - openapi/fiserv-bankinghub-openapi.yml\n  - openapi/fiserv-carddeveloper-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using the CardPointe Gateway credentials.\n  sources:\n  - openapi/fiserv-cardpointe-gateway-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: API key provided by Fiserv for authenticating requests.\n  sources:\n  - openapi/fiserv-commercehub-openapi.yml\n- name: hmacAuth\n  type: apiKey\n  in: header\n  parameter:\
  \ Authorization\n  description: HMAC signature generated using the API secret, request timestamp, and request\n    payload for message integrity verification.\n  sources:\n  - openapi/fiserv-commercehub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiserv/refs/heads/main/authentication/fiserv-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Banking
- Financial
- Payments
- Wealth Management
- Fortune 500
---
