---
api_key_in:
- header
api_specs:
- filename: securonix-policy-management-api.json
  format: json
  label: Securonix Policy Management API
  slug: securonix-policy-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securonix/refs/heads/main/openapi/securonix-policy-management-api.json
- filename: securonix-datasource-onboarding-api.json
  format: json
  label: Securonix Datasource Onboarding API
  slug: securonix-datasource-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securonix/refs/heads/main/openapi/securonix-datasource-onboarding-api.json
- filename: securonix-device-monitoring-api.json
  format: json
  label: Securonix Device Monitoring API
  slug: securonix-device-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securonix/refs/heads/main/openapi/securonix-device-monitoring-api.json
- filename: securonix-threatq-api.json
  format: json
  label: Securonix ThreatQ API
  slug: securonix-threatq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securonix/refs/heads/main/openapi/securonix-threatq-api.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Securonix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Securonix secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Securonix
provider_slug: securonix
scheme_count: 3
schemes:
- in: header
  name: ApiKeyAuth
  parameter: wstoken
  sources:
  - openapi/securonix-datasource-onboarding-api.json
  type: apiKey
- description: Authentication token.
  in: header
  name: tokenAuth
  parameter: token
  sources:
  - openapi/securonix-device-monitoring-api.json
  type: apiKey
- bearerFormat: JWT
  description: "**Authentication**\n- The JWT is issued using the `wstoken` (obtained after successful authentication).\n- A valid JWT token must be provided via `Authorization: Bearer <token>`.  \n\n**Authorization**:\n- API access is controlled by validating the `role` and `tenant` claims from the JWT.   \n- All **read** APIs require one of the following roles: `ROLE_ADMIN`, `ROLE_CONTENT_DEVELOPER`, `ROLE_READ_ONLY`"
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/securonix-policy-management-api.json
  - openapi/securonix-threatq-api.json
  type: http
slug: securonix-authentication
source_filename: securonix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/securonix-datasource-onboarding-api.json, openapi/securonix-device-monitoring-api.json,\n  openapi/securonix-policy-management-api.json, openapi/securonix-threatq-api.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: wstoken\n  sources:\n  - openapi/securonix-datasource-onboarding-api.json\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: token\n  description: Authentication token.\n  sources:\n  - openapi/securonix-device-monitoring-api.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: \"**Authentication**\\n- The JWT is issued using the `wstoken` (obtained after\\\n    \\ successful authentication).\\n- A valid JWT token must be provided via `Authorization:\\\n    \\ Bearer <token>`.  \\n\\n**Authorization**:\\n- API access is controlled by validating the\\\n   \
  \ \\ `role` and `tenant` claims from the JWT.   \\n- All **read** APIs require one of the following\\\n    \\ roles: `ROLE_ADMIN`, `ROLE_CONTENT_DEVELOPER`, `ROLE_READ_ONLY`\"\n  sources:\n  - openapi/securonix-policy-management-api.json\n  - openapi/securonix-threatq-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/securonix/refs/heads/main/authentication/securonix-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Security
- SIEM
- UEBA
- SOAR
- Threat Intelligence
- Security Analytics
- Cybersecurity
- Log Management
- Detection and Response
- MITRE ATT&CK
---
