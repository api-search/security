---
api_key_in:
- header
api_specs:
- filename: halo-connect-fhir-api-openapi.yml
  format: yaml
  label: Halo Connect FHIR API
  slug: halo-connect-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halo-connect/refs/heads/main/openapi/halo-connect-fhir-api-openapi.yml
- filename: halo-connect-registered-queries-api-openapi.yml
  format: yaml
  label: Halo Connect Registered Queries API
  slug: halo-connect-registered-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halo-connect/refs/heads/main/openapi/halo-connect-registered-queries-api-openapi.yml
- filename: halo-connect-sites-api-openapi.yml
  format: yaml
  label: Halo Connect Sites API
  slug: halo-connect-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halo-connect/refs/heads/main/openapi/halo-connect-sites-api-openapi.yml
- filename: halo-connect-sql-passthrough-api-openapi.yml
  format: yaml
  label: Halo Connect SQL Passthrough API
  slug: halo-connect-sql-passthrough-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halo-connect/refs/heads/main/openapi/halo-connect-sql-passthrough-api-openapi.yml
- filename: halo-connect-tokens-api-openapi.yml
  format: yaml
  label: Halo Connect Tokens API
  slug: halo-connect-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halo-connect/refs/heads/main/openapi/halo-connect-tokens-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Halo Connect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Halo Connect secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Halo Connect
provider_slug: halo-connect
scheme_count: 3
schemes:
- description: The subscription key for the API.
  in: header
  name: SubscriptionKey
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/halo-connect-desktop-openapi.json
  - openapi/halo-connect-integrator-openapi.json
  type: apiKey
- bearerFormat: JWT
  description: Bearer token for authentication.
  name: AuthorizationHeader
  scheme: bearer
  sources:
  - openapi/halo-connect-desktop-openapi.json
  type: http
- description: Device ID of the device making the request.
  in: header
  name: DeviceIdHeader
  parameter: DeviceId
  sources:
  - openapi/halo-connect-desktop-openapi.json
  type: apiKey
slug: halo-connect-authentication
source_filename: halo-connect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/halo-connect-desktop-openapi.json, openapi/halo-connect-integrator-openapi.json\ndocs: https://docs.haloconnect.io/halo-cloud/getting-started/\nnotes: >-\n  Integrator API authenticates with an Azure API Management subscription key\n  (Ocp-Apim-Subscription-Key header). Desktop API additionally requires a bearer\n  JWT (obtained from POST /integrator/token using integrator auth) plus a DeviceId\n  header. There is no OAuth 2.0 / OIDC flow and no self-serve public sign-up; keys\n  are issued per approved integrator and are environment-scoped (stage vs production).\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: SubscriptionKey\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  description: The subscription key for the API.\n  sources:\n  - openapi/halo-connect-desktop-openapi.json\n  - openapi/halo-connect-integrator-openapi.json\n- name: AuthorizationHeader\n\
  \  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token for authentication.\n  sources:\n  - openapi/halo-connect-desktop-openapi.json\n- name: DeviceIdHeader\n  type: apiKey\n  in: header\n  parameter: DeviceId\n  description: Device ID of the device making the request.\n  sources:\n  - openapi/halo-connect-desktop-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/halo-connect/refs/heads/main/authentication/halo-connect-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Healthcare
- Australia
- FHIR
- HL7
- Interoperability
- EHR
- Practice Management
- Primary Care
- AU Base
- Health Data
---
