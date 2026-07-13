---
api_key_in:
- cookie
api_specs:
- filename: agstack-openagri-weather-service-openapi.yml
  format: yaml
  label: OpenAgri Weather Service
  slug: openagri-weather-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/openapi/agstack-openagri-weather-service-openapi.yml
- filename: agstack-openagri-farm-calendar-openapi.yml
  format: yaml
  label: OpenAgri Farm Calendar
  slug: openagri-farm-calendar
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/openapi/agstack-openagri-farm-calendar-openapi.yml
- filename: agstack-asset-registry-openapi.yml
  format: yaml
  label: AgStack Asset Registry
  slug: asset-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/openapi/agstack-asset-registry-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Agstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgStack Foundation secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AgStack Foundation
provider_slug: agstack
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: '**Required for most operations.**

    1. Login via `/login` to get token.

    2. Paste access token here.'
  name: Bearer_Token
  scheme: bearer
  sources:
  - openapi/agstack-asset-registry-openapi.yml
  - openapi/agstack-openagri-weather-service-openapi.yml
  type: http
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/agstack-openagri-farm-calendar-openapi.yml
  type: apiKey
slug: agstack-authentication
source_filename: agstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agstack-asset-registry-openapi.yml, openapi/agstack-openagri-farm-calendar-openapi.yml,\n  openapi/agstack-openagri-weather-service-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: Bearer_Token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    **Required for most operations.**\n    1. Login via `/login` to get token.\n    2. Paste access token here.\n  sources:\n  - openapi/agstack-asset-registry-openapi.yml\n  - openapi/agstack-openagri-weather-service-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/agstack-openagri-farm-calendar-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/authentication/agstack-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
---
