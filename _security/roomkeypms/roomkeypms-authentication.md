---
api_key_in:
- query
api_specs:
- filename: roomkeypms-openapi.yml
  format: yaml
  label: RoomKeyPMS Reservation Data API
  slug: roomkeypms-reservation-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roomkeypms/refs/heads/main/openapi/roomkeypms-openapi.yml
- filename: roomkeypms-openapi.yml
  format: yaml
  label: RoomKeyPMS POS Integration API
  slug: roomkeypms-pos-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roomkeypms/refs/heads/main/openapi/roomkeypms-openapi.yml
- filename: roomkeypms-openapi.yml
  format: yaml
  label: RoomKeyPMS Statistics and Forecasts API
  slug: roomkeypms-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roomkeypms/refs/heads/main/openapi/roomkeypms-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Roomkeypms Authentication
name_suffix: Authentication
oauth_flows: []
overview: RoomKeyPMS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RoomKeyPMS
provider_slug: roomkeypms
scheme_count: 1
schemes:
- description: API key issued by RoomKeyPMS after a hotel's IT team requests access and the property signs off.
  in: query
  name: apiKeyAuth
  parameter: key
  sources:
  - openapi/roomkeypms-openapi.yml
  type: apiKey
slug: roomkeypms-authentication
source_filename: roomkeypms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/roomkeypms-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key issued by RoomKeyPMS after a hotel's IT team requests access and the\n    property signs off.\n  sources:\n  - openapi/roomkeypms-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roomkeypms/refs/heads/main/authentication/roomkeypms-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Hospitality
- Hotel Technology
- Property Management System
- PMS
- Reservations
- POS
- Gated API
---
