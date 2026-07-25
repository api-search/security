---
api_key_in:
- header
api_specs:
- filename: channex-ari-api-openapi.yml
  format: yaml
  label: Channex ARI API
  slug: channex-ari-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channex/refs/heads/main/openapi/channex-ari-api-openapi.yml
- filename: channex-bookings-api-openapi.yml
  format: yaml
  label: Channex Bookings API
  slug: channex-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channex/refs/heads/main/openapi/channex-bookings-api-openapi.yml
- filename: channex-channels-api-openapi.yml
  format: yaml
  label: Channex Channels API
  slug: channex-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channex/refs/heads/main/openapi/channex-channels-api-openapi.yml
- filename: channex-properties-api-openapi.yml
  format: yaml
  label: Channex Properties API
  slug: channex-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channex/refs/heads/main/openapi/channex-properties-api-openapi.yml
- filename: channex-rate-plans-api-openapi.yml
  format: yaml
  label: Channex Rate Plans API
  slug: channex-rate-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channex/refs/heads/main/openapi/channex-rate-plans-api-openapi.yml
- filename: channex-room-types-api-openapi.yml
  format: yaml
  label: Channex Room Types API
  slug: channex-room-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channex/refs/heads/main/openapi/channex-room-types-api-openapi.yml
- filename: channex-webhooks-api-openapi.yml
  format: yaml
  label: Channex Webhooks API
  slug: channex-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channex/refs/heads/main/openapi/channex-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Channex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Channex secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Channex
provider_slug: channex
scheme_count: 1
schemes:
- description: Channex API key passed in the `user-api-key` request header. Generate a key in the Channex application under your account settings.
  in: header
  name: userApiKey
  parameter: user-api-key
  sources:
  - openapi/channex-openapi.yml
  type: apiKey
slug: channex-authentication
source_filename: channex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/channex-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: userApiKey\n  type: apiKey\n  in: header\n  parameter: user-api-key\n  description: Channex API key passed in the `user-api-key` request header. Generate a key in\n    the Channex application under your account settings.\n  sources:\n  - openapi/channex-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channex/refs/heads/main/authentication/channex-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Hospitality
- Channel Manager
- Hotel Distribution
- OTA
- Bookings
---
