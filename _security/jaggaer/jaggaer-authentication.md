---
api_key_in:
- header
api_specs:
- filename: jaggaer-aso-ches-openapi.yml
  format: yaml
  label: JAGGAER ASO Customer Host Entity Service API
  slug: jaggaer-aso-customer-host-entity-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-aso-ches-openapi.yml
- filename: jaggaer-aso-ees-openapi.yml
  format: yaml
  label: JAGGAER ASO Event Entity Service API
  slug: jaggaer-aso-event-entity-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-aso-ees-openapi.yml
- filename: jaggaer-aso-quay-openapi.yml
  format: yaml
  label: JAGGAER ASO Quay Optimization API
  slug: jaggaer-aso-quay-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-aso-quay-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jaggaer Authentication
name_suffix: Authentication
oauth_flows: []
overview: JAGGAER secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: JAGGAER
provider_slug: jaggaer
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token for authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/jaggaer-aso-ches-openapi.yml
  - openapi/jaggaer-aso-ees-openapi.yml
  type: http
- description: API key passed as a request header.
  in: header
  name: apiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/jaggaer-aso-ches-openapi.yml
  - openapi/jaggaer-aso-ees-openapi.yml
  - openapi/jaggaer-aso-quay-openapi.yml
  type: apiKey
slug: jaggaer-authentication
source_filename: jaggaer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jaggaer-aso-ches-openapi.yml, openapi/jaggaer-aso-ees-openapi.yml, openapi/jaggaer-aso-quay-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token for authentication.\n  sources:\n  - openapi/jaggaer-aso-ches-openapi.yml\n  - openapi/jaggaer-aso-ees-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key passed as a request header.\n  sources:\n  - openapi/jaggaer-aso-ches-openapi.yml\n  - openapi/jaggaer-aso-ees-openapi.yml\n  - openapi/jaggaer-aso-quay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/authentication/jaggaer-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Procurement
- Sourcing
- Supplier Management
- Contracts
- Spend Analytics
- eProcurement
- Source-to-Pay
- Procure-to-Pay
---
