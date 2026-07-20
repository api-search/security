---
api_key_in:
- header
api_specs:
- filename: capmo-rest-api-openapi-original.json
  format: json
  label: Capmo REST API
  slug: capmo-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capmo/refs/heads/main/openapi/capmo-rest-api-openapi-original.json
- filename: capmo-webhook-api-openapi-original.json
  format: json
  label: Capmo Webhook API
  slug: capmo-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capmo/refs/heads/main/openapi/capmo-webhook-api-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Capmo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capmo secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Capmo
provider_slug: capmo
scheme_count: 2
schemes:
- description: 'For authentication, use the custom prefix followed by a space and then your API key. Example: "Capmo YOUR_API_KEY".'
  in: header
  name: CapmoAuth
  parameter: Authorization
  sources:
  - openapi/capmo-rest-api-openapi-original.json
  type: apiKey
- description: HMAC SHA256 signature calculated using the registered secret and the raw request body to verify authenticity. The value should be prefixed with `sha256=`.
  in: header
  name: WebhookSignature
  parameter: X-Capmo-Signature
  sources:
  - openapi/capmo-webhook-api-openapi-original.json
  type: apiKey
slug: capmo-authentication
source_filename: capmo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/capmo-rest-api-openapi-original.json, openapi/capmo-webhook-api-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: CapmoAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'For authentication, use the custom prefix followed by a space and then your\n    API key. Example: \"Capmo YOUR_API_KEY\".'\n  sources:\n  - openapi/capmo-rest-api-openapi-original.json\n- name: WebhookSignature\n  type: apiKey\n  in: header\n  parameter: X-Capmo-Signature\n  description: HMAC SHA256 signature calculated using the registered secret and the raw request\n    body to verify authenticity. The value should be prefixed with `sha256=`.\n  sources:\n  - openapi/capmo-webhook-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capmo/refs/heads/main/authentication/capmo-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Vertical Software
- Construction
- Project Management
- Construction Tech
- Field Management
- Building
- DACH
---
