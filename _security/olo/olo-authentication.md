---
api_key_in:
- header
api_specs:
- filename: olo-ordering-openapi.yml
  format: yaml
  label: Olo Ordering API
  slug: olo-ordering
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/olo/refs/heads/main/openapi/olo-ordering-openapi.yml
- filename: olo-ordering-openapi.yml
  format: yaml
  label: Olo Rails API
  slug: olo-rails
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/olo/refs/heads/main/openapi/olo-ordering-openapi.yml
- filename: olo-promotions-openapi.yml
  format: yaml
  label: Olo Loyalty API
  slug: olo-loyalty
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/olo/refs/heads/main/openapi/olo-promotions-openapi.yml
- filename: olo-webhooks-asyncapi.yml
  format: yaml
  label: Olo Webhooks
  slug: olo-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/olo/refs/heads/main/asyncapi/olo-webhooks-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Olo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Olo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Olo
provider_slug: olo
scheme_count: 1
schemes:
- description: HMAC-SHA256 signature authorization. The signed message is the newline-joined concatenation of clientId, HTTP verb, content type, base64-encoded SHA-256 hash of the request body, path and query, and the RFC 1123 timestamp. The result is base64-encoded and sent as "OloSignature {clientId}:{signature}" in the Authorization header, with the matching timestamp in the Date header.
  in: header
  name: OloSignature
  parameter: Authorization
  sources:
  - openapi/olo-ordering-openapi.yml
  - openapi/olo-promotions-openapi.yml
  type: apiKey
slug: olo-authentication
source_filename: olo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/olo-ordering-openapi.yml, openapi/olo-promotions-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: OloSignature\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: HMAC-SHA256 signature authorization. The signed message is the newline-joined\n    concatenation of clientId, HTTP verb, content type, base64-encoded SHA-256 hash of the request\n    body, path and query, and the RFC 1123 timestamp. The result is base64-encoded and sent\n    as \"OloSignature {clientId}:{signature}\" in the Authorization header, with the matching\n    timestamp in the Date header.\n  sources:\n  - openapi/olo-ordering-openapi.yml\n  - openapi/olo-promotions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olo/refs/heads/main/authentication/olo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Food Service
- Restaurants
- Online Ordering
- Delivery
- Point of Sale
- Hospitality
- Payments
- Loyalty
- Marketing
---
