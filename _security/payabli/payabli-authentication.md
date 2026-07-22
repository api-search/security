---
api_key_in:
- header
api_specs:
- filename: payabli-api-reference-openapi.json
  format: json
  label: Payabli API
  slug: payabli-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payabli/refs/heads/main/openapi/payabli-api-reference-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Payabli Authentication
name_suffix: Authentication
oauth_flows: []
overview: Payabli secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Payabli
provider_slug: payabli
scheme_count: 2
schemes:
- description: OAuth2 Bearer access token from the client-credentials flow. See [OAuth authentication](/developers/oauth-authentication).
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/payabli-api-reference-openapi.json
  type: http
- description: Long-lived API token sent in the `requestToken` header. See [API token authentication](/developers/api-tokens).
  in: header
  name: APIKeyAuth
  parameter: requestToken
  sources:
  - openapi/payabli-api-reference-openapi.json
  type: apiKey
slug: payabli-authentication
source_filename: payabli-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/payabli-api-reference-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth2 Bearer access token from the client-credentials flow. See [OAuth authentication](/developers/oauth-authentication).\n  sources:\n  - openapi/payabli-api-reference-openapi.json\n- name: APIKeyAuth\n  type: apiKey\n  in: header\n  parameter: requestToken\n  description: Long-lived API token sent in the `requestToken` header. See [API token authentication](/developers/api-tokens).\n  sources:\n  - openapi/payabli-api-reference-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payabli/refs/heads/main/authentication/payabli-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Payments
- Embedded Payments
- Fintech
- Payment Processing
- Payments API
- Payouts
- Billing
- ACH
- Cards
- Tokenization
- Webhooks
---
