---
api_key_in: []
api_specs:
- filename: human-api-admin-order-types-openapi.json
  format: json
  label: Human API Admin API
  slug: human-api-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/openapi/human-api-admin-order-types-openapi.json
- filename: human-api-auth-admin-token-openapi.json
  format: json
  label: Human API Authentication API
  slug: human-api-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/openapi/human-api-auth-admin-token-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Human Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Human API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Human API
provider_slug: human-api
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/human-api-admin-order-types-openapi.json
  - openapi/human-api-admin-user-reports-openapi.json
  - openapi/human-api-admin-users-list-openapi.json
  type: http
slug: human-api-authentication
source_filename: human-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/human-api-admin-order-types-openapi.json, openapi/human-api-admin-user-reports-openapi.json,\n  openapi/human-api-admin-users-list-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/human-api-admin-order-types-openapi.json\n  - openapi/human-api-admin-user-reports-openapi.json\n  - openapi/human-api-admin-users-list-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/authentication/human-api-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- United States
- Health Data
- EHR
- Interoperability
- Remote Monitoring
- Wearables
- Life Insurance
- Clinical Data
- Health API
---
