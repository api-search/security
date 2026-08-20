---
api_key_in:
- header
api_specs:
- filename: luma-calendars-api-openapi.yml
  format: yaml
  label: Luma Calendars API
  slug: luma-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma/refs/heads/main/openapi/luma-calendars-api-openapi.yml
- filename: luma-events-api-openapi.yml
  format: yaml
  label: Luma Events API
  slug: luma-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma/refs/heads/main/openapi/luma-events-api-openapi.yml
- filename: luma-memberships-api-openapi.yml
  format: yaml
  label: Luma Memberships API
  slug: luma-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma/refs/heads/main/openapi/luma-memberships-api-openapi.yml
- filename: luma-miscellaneous-api-openapi.yml
  format: yaml
  label: Luma Miscellaneous API
  slug: luma-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma/refs/heads/main/openapi/luma-miscellaneous-api-openapi.yml
- filename: luma-organizations-api-openapi.yml
  format: yaml
  label: Luma Organizations API
  slug: luma-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma/refs/heads/main/openapi/luma-organizations-api-openapi.yml
- filename: luma-webhooks-api-openapi.yml
  format: yaml
  label: Luma Webhooks API
  slug: luma-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma/refs/heads/main/openapi/luma-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Luma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Luma secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Luma
provider_slug: luma
scheme_count: 1
schemes:
- description: API key to authenticate requests to the Luma API. Generate an API key on your Luma dashboard.
  in: header
  name: apiKeyAuth
  parameter: x-luma-api-key
  sources:
  - openapi/openapi.json
  type: apiKey
slug: luma-authentication
source_filename: luma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-luma-api-key\n  description: API key to authenticate requests to the Luma API. Generate an API key on your\n    Luma dashboard.\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luma/refs/heads/main/authentication/luma-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Event
- Event Management
- Ticketing
- Community
- Calendars
- Guests
- Attendance
---
