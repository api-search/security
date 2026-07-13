---
api_key_in:
- header
api_specs:
- filename: swetrix-events-api-openapi.yml
  format: yaml
  label: Swetrix Events API
  slug: swetrix-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-events-api-openapi.yml
- filename: swetrix-statistics-api-openapi.yml
  format: yaml
  label: Swetrix Statistics API
  slug: swetrix-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-statistics-api-openapi.yml
- filename: swetrix-admin-api-openapi.yml
  format: yaml
  label: Swetrix Admin API
  slug: swetrix-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-admin-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Swetrix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swetrix secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Swetrix
provider_slug: swetrix
scheme_count: 1
schemes:
- description: API key from Swetrix account settings (https://swetrix.com/user-settings)
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/swetrix-admin-api-openapi.yml
  - openapi/swetrix-events-api-openapi.yml
  - openapi/swetrix-statistics-api-openapi.yml
  type: apiKey
slug: swetrix-authentication
source_filename: swetrix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/swetrix-admin-api-openapi.yml, openapi/swetrix-events-api-openapi.yml, openapi/swetrix-statistics-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key from Swetrix account settings (https://swetrix.com/user-settings)\n  sources:\n  - openapi/swetrix-admin-api-openapi.yml\n  - openapi/swetrix-events-api-openapi.yml\n  - openapi/swetrix-statistics-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/authentication/swetrix-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Cookieless Tracking
- GDPR Compliant
- Open Source
- Privacy
- Real-Time Analytics
- Web Analytics
---
