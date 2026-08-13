---
api_key_in:
- cookie
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nickelytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nickelytics secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nickelytics
provider_slug: nickelytics
scheme_count: 2
schemes:
- description: API Key authentication via cookie
  in: cookie
  name: apiKeyCookie
  parameter: apiKeyCookie
  sources:
  - openapi/nickelytics-rads-auth-openapi.json
  type: apiKey
- description: Bearer token authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nickelytics-rads-auth-openapi.json
  type: http
slug: nickelytics-authentication
source_filename: nickelytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/nickelytics-rads-auth-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: apiKeyCookie\n  type: apiKey\n  in: cookie\n  parameter: apiKeyCookie\n  description: API Key authentication via cookie\n  sources:\n  - openapi/nickelytics-rads-auth-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication\n  sources:\n  - openapi/nickelytics-rads-auth-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nickelytics/refs/heads/main/authentication/nickelytics-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Advertising
- OOH
- DOOH
- Programmatic Advertising
- Mobility
- Robotics
- Rideshare
- AdTech
- Authentication
---
