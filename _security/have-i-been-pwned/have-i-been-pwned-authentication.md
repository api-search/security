---
api_key_in:
- header
api_specs:
- filename: have-i-been-pwned-openapi.json
  format: json
  label: Have I Been Pwned API v3
  slug: api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/openapi/have-i-been-pwned-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Have I Been Pwned Authentication
name_suffix: Authentication
oauth_flows: []
overview: Have I Been Pwned secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Have I Been Pwned
provider_slug: have-i-been-pwned
scheme_count: 1
schemes:
- description: HIBP API key passed in the hibp-api-key header. Paid APIs require a 32-character hexadecimal value. On supported test-only endpoints, any 32-character hexadecimal value can be used as a test key for the hibp-integration-tests.com domain.
  in: header
  name: HibpApiKey
  parameter: hibp-api-key
  sources:
  - openapi/have-i-been-pwned-openapi.json
  type: apiKey
slug: have-i-been-pwned-authentication
source_filename: have-i-been-pwned-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/have-i-been-pwned-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: HibpApiKey\n  type: apiKey\n  in: header\n  parameter: hibp-api-key\n  description: HIBP API key passed in the hibp-api-key header. Paid APIs require a 32-character\n    hexadecimal value. On supported test-only endpoints, any 32-character hexadecimal value\n    can be used as a test key for the hibp-integration-tests.com domain.\n  sources:\n  - openapi/have-i-been-pwned-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/authentication/have-i-been-pwned-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- Data Breaches
- Pwned Passwords
- Identity
- Threat Intelligence
- Credential Stuffing
---
