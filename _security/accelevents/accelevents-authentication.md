---
api_key_in:
- header
api_specs:
- filename: accelevents-openapi.yml
  format: yaml
  label: Accelevents Events API
  slug: accelevents-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/openapi/accelevents-openapi.yml
- filename: accelevents-openapi.yml
  format: yaml
  label: Accelevents Attendees API
  slug: accelevents-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/openapi/accelevents-openapi.yml
- filename: accelevents-openapi.yml
  format: yaml
  label: Accelevents Ticketing Orders API
  slug: accelevents-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/openapi/accelevents-openapi.yml
- filename: accelevents-openapi.yml
  format: yaml
  label: Accelevents Tickets API
  slug: accelevents-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/openapi/accelevents-openapi.yml
- filename: accelevents-openapi.yml
  format: yaml
  label: Accelevents Sessions API
  slug: accelevents-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/openapi/accelevents-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Accelevents Authentication
name_suffix: Authentication
oauth_flows: []
overview: Accelevents secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Accelevents
provider_slug: accelevents
scheme_count: 1
schemes:
- description: Organization API key generated from the account Integrations tab (Edit Enterprise -> Integrations -> API Key), passed in a request header. The header name is modeled as "AUTHENTICATION" per the getting-started guide; confirm the exact name and format on the API reference before use.
  in: header
  name: apiKeyAuth
  parameter: AUTHENTICATION
  sources:
  - openapi/accelevents-openapi.yml
  type: apiKey
slug: accelevents-authentication
source_filename: accelevents-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/accelevents-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: AUTHENTICATION\n  description: Organization API key generated from the account Integrations tab (Edit Enterprise\n    -> Integrations -> API Key), passed in a request header. The header name is modeled as \"AUTHENTICATION\"\n    per the getting-started guide; confirm the exact name and format on the API reference before\n    use.\n  sources:\n  - openapi/accelevents-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/authentication/accelevents-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Event Management
- Ticketing
- Events
- Registration
- Virtual Events
- Sessions
---
