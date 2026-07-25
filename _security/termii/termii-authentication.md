---
api_key_in:
- query
api_specs:
- filename: termii-campaigns-api-openapi.yml
  format: yaml
  label: Termii Campaigns API
  slug: termii-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-campaigns-api-openapi.yml
- filename: termii-contacts-api-openapi.yml
  format: yaml
  label: Termii Contacts API
  slug: termii-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-contacts-api-openapi.yml
- filename: termii-insights-api-openapi.yml
  format: yaml
  label: Termii Insights API
  slug: termii-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-insights-api-openapi.yml
- filename: termii-messaging-api-openapi.yml
  format: yaml
  label: Termii Messaging API
  slug: termii-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-messaging-api-openapi.yml
- filename: termii-sender-ids-api-openapi.yml
  format: yaml
  label: Termii Sender IDs API
  slug: termii-sender-ids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-sender-ids-api-openapi.yml
- filename: termii-token-api-openapi.yml
  format: yaml
  label: Termii Token API
  slug: termii-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-token-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Termii Authentication
name_suffix: Authentication
oauth_flows: []
overview: Termii secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Termii
provider_slug: termii
scheme_count: 1
schemes:
- description: Termii authenticates every request with an api_key. For GET requests it is passed as the api_key query parameter; for POST, PATCH, and DELETE requests it is included in the JSON request body.
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/termii-openapi.yml
  type: apiKey
slug: termii-authentication
source_filename: termii-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/termii-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Termii authenticates every request with an api_key. For GET requests it is passed\n    as the api_key query parameter; for POST, PATCH, and DELETE requests it is included in the\n    JSON request body.\n  sources:\n  - openapi/termii-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/authentication/termii-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Messaging
- SMS
- OTP
- WhatsApp
- Verification
---
