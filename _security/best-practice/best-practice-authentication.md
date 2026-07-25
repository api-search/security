---
api_key_in:
- header
api_specs:
- filename: haloconnect-integrator-openapi.json
  format: json
  label: Halo Cloud API for Integrators
  slug: halo-cloud-integrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-practice/refs/heads/main/openapi/haloconnect-integrator-openapi.json
- filename: haloconnect-desktop-openapi.json
  format: json
  label: Halo Cloud API for Desktop Applications
  slug: halo-cloud-desktop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-practice/refs/heads/main/openapi/haloconnect-desktop-openapi.json
- filename: haloconnect-integrator-openapi.json
  format: json
  label: FHIR API for Bp Premier
  slug: fhir-api-bp-premier
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-practice/refs/heads/main/openapi/haloconnect-integrator-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Best Practice Authentication
name_suffix: Authentication
oauth_flows: []
overview: Best Practice Software secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Best Practice Software
provider_slug: best-practice
scheme_count: 3
schemes:
- description: The subscription key for the API.
  in: header
  name: SubscriptionKey
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/haloconnect-desktop-openapi.json
  - openapi/haloconnect-integrator-openapi.json
  type: apiKey
- bearerFormat: JWT
  description: Bearer token for authentication.
  name: AuthorizationHeader
  scheme: bearer
  sources:
  - openapi/haloconnect-desktop-openapi.json
  type: http
- description: Device ID of the device making the request.
  in: header
  name: DeviceIdHeader
  parameter: DeviceId
  sources:
  - openapi/haloconnect-desktop-openapi.json
  type: apiKey
slug: best-practice-authentication
source_filename: best-practice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/haloconnect-desktop-openapi.json, openapi/haloconnect-integrator-openapi.json\ndocs: https://docs.haloconnect.io/halo-cloud/getting-started/\nnotes: >-\n  Integrator API authenticates with an Azure API Management subscription key\n  (Ocp-Apim-Subscription-Key header). Desktop apps additionally supply a bearer JWT\n  (obtained from obtainToken, expires and must be renewed) plus a DeviceId header. Every\n  site-scoped call also requires an active pairing with the target site. No OAuth2/OIDC.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: SubscriptionKey\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  description: The subscription key for the API.\n  sources:\n  - openapi/haloconnect-desktop-openapi.json\n  - openapi/haloconnect-integrator-openapi.json\n- name: AuthorizationHeader\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer\
  \ token for authentication.\n  sources:\n  - openapi/haloconnect-desktop-openapi.json\n- name: DeviceIdHeader\n  type: apiKey\n  in: header\n  parameter: DeviceId\n  description: Device ID of the device making the request.\n  sources:\n  - openapi/haloconnect-desktop-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/best-practice/refs/heads/main/authentication/best-practice-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Healthcare
- Australia
- EHR
- EMR
- FHIR
- HL7
- Interoperability
- AU Base
- Practice Management
- General Practice
- Appointments
- Scheduling
---
