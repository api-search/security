---
api_key_in: []
api_specs:
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage SMS API
  slug: vonage-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage Voice API
  slug: vonage-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage Messages API
  slug: vonage-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage Verify API
  slug: vonage-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage Numbers API
  slug: vonage-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage Application API
  slug: vonage-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vonage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vonage secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vonage
provider_slug: vonage
scheme_count: 2
schemes:
- description: Base64-encoded API key and secret joined by a colon.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/vonage-openapi.yml
  type: http
- bearerFormat: JWT
  description: JWT token for application-level authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vonage-openapi.yml
  type: http
slug: vonage-authentication
source_filename: vonage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vonage-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Base64-encoded API key and secret joined by a colon.\n  sources:\n  - openapi/vonage-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token for application-level authentication.\n  sources:\n  - openapi/vonage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/authentication/vonage-authentication.yml
summary_line: http · 2 schemes
tags:
- Communication
- Messaging
- Telecommunications
- Video Conferencing
- Voice
- SMS
- Verification
---
