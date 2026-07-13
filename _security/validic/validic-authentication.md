---
api_key_in:
- query
api_specs:
- filename: validic-openapi.yml
  format: yaml
  label: Validic Users API
  slug: validic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-openapi.yml
- filename: validic-openapi.yml
  format: yaml
  label: Validic Marketplace & Connections API
  slug: validic-marketplace-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-openapi.yml
- filename: validic-openapi.yml
  format: yaml
  label: Validic Observations & Data API
  slug: validic-observations-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-openapi.yml
- filename: validic-openapi.yml
  format: yaml
  label: Validic Devices API
  slug: validic-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-openapi.yml
- filename: validic-openapi.yml
  format: yaml
  label: Validic Streaming API
  slug: validic-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-openapi.yml
- filename: validic-openapi.yml
  format: yaml
  label: Validic Push Service API
  slug: validic-push-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Validic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Validic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Validic
provider_slug: validic
scheme_count: 1
schemes:
- description: Organization access token passed as the `token` query parameter.
  in: query
  name: tokenAuth
  parameter: token
  sources:
  - openapi/validic-openapi.yml
  type: apiKey
slug: validic-authentication
source_filename: validic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/validic-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: Organization access token passed as the `token` query parameter.\n  sources:\n  - openapi/validic-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/authentication/validic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Health Data
- Digital Health
- Wearables
- Remote Patient Monitoring
- Health IoT
- Interoperability
- HIPAA
---
