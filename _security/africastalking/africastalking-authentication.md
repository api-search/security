---
api_key_in:
- header
api_specs:
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking SMS API
  slug: sms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking USSD API
  slug: ussd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking Voice API
  slug: voice
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking Airtime API
  slug: airtime
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking Mobile Data API
  slug: mobile-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Africastalking Authentication
name_suffix: Authentication
oauth_flows: []
overview: Africa's Talking secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Africa's Talking
provider_slug: africastalking
scheme_count: 1
schemes:
- description: Africa's Talking API key generated from your account dashboard.
  in: header
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/africastalking-openapi.yml
  type: apiKey
slug: africastalking-authentication
source_filename: africastalking-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/africastalking-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apiKey\n  description: Africa's Talking API key generated from your account dashboard.\n  sources:\n  - openapi/africastalking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/authentication/africastalking-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Communications
- SMS
- USSD
- Voice
- Airtime
- Mobile Data
- Payments
- Africa
---
