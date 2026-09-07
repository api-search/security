---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: xrhealth-platform-openapi.yml
  format: yaml
  label: XRHealth Platform API
  slug: xrhealth-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrhealth/refs/heads/main/openapi/xrhealth-platform-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Xrhealth Authentication
name_suffix: Authentication
oauth_flows: []
overview: XRHealth secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: XRHealth
provider_slug: xrhealth
scheme_count: 2
schemes:
- in: header
  name: applicationToken
  parameter: X-XRHealth-Application-Token
  sources:
  - openapi/xrhealth-platform-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: patientBearer
  scheme: bearer
  sources:
  - openapi/xrhealth-platform-openapi.yml
  type: http
slug: xrhealth-authentication
source_filename: xrhealth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: derived\nsource: openapi/xrhealth-platform-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: applicationToken\n  type: apiKey\n  in: header\n  parameter: X-XRHealth-Application-Token\n  sources:\n  - openapi/xrhealth-platform-openapi.yml\n- name: patientBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/xrhealth-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xrhealth/refs/heads/main/authentication/xrhealth-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Health
- Digital Health
- Telehealth
- Virtual Reality
- Extended Reality
- Medical Devices
- Rehabilitation
- Mental Health
- Patient Authentication
- Healthcare
---
