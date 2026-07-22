---
api_key_in:
- header
api_specs:
- filename: nexhealth-openapi-original.json
  format: json
  label: NexHealth Synchronizer API
  slug: nexhealth-synchronizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexhealth/refs/heads/main/openapi/nexhealth-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nexhealth Authentication
name_suffix: Authentication
oauth_flows: []
overview: NexHealth secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NexHealth
provider_slug: nexhealth
scheme_count: 1
schemes:
- in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/nexhealth-openapi-original.json
  type: apiKey
slug: nexhealth-authentication
source_filename: nexhealth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nexhealth-openapi-original.json\ndocs: https://docs.nexhealth.com/reference/authentication-1\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: api-key-exchanged-for-bearer-jwt\nschemes:\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/nexhealth-openapi-original.json\nflow:\n  description: \"Request an API key via the developer portal, then POST it in the Authorization header to /authenticates to receive a short-lived bearer JWT used on all other routes. Every request must also send the Nex-Api-Version header.\"\n  steps:\n  - Obtain an API key from the NexHealth Developer Portal (test key self-serve; production via request-access).\n  - \"POST /authenticates with header 'Authorization: <API_KEY>' and 'Nex-Api-Version: v3.0.0'.\"\n  - Read the returned data.token (a JSON Web Token).\n  - \"Send 'Authorization: Bearer <token>' on all subsequent\
  \ requests.\"\n  token:\n    type: bearer-jwt\n    format: JWT\n    lifetime_production: 1 hour\n    lifetime_sandbox: 24 hours\n    exchange_operation: postAuthenticates\n  required_headers:\n  - Authorization\n  - Nex-Api-Version\n  key_provisioning:\n    test_key: https://developers.nexhealth.com/test/api-key\n    production_access: https://www.nexhealth.com/api-request/request-access\n  unauthenticated_response: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexhealth/refs/heads/main/authentication/nexhealth-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Healthcare
- EHR
- Practice Management
- Scheduling
- Appointments
- Dental
- Patients
- Health Records
- Insurance
- Webhooks
---
