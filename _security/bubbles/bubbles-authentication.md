---
api_key_in: []
api_specs:
- filename: bubbles-openapi.yml
  format: yaml
  label: Bubble Data API
  slug: bubble-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bubbles/refs/heads/main/openapi/bubbles-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bubbles Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bubble secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bubble
provider_slug: bubbles
scheme_count: 1
schemes:
- description: Bearer token issued in the Bubble app's Settings → API tab.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bubbles-openapi.yml
  type: http
slug: bubbles-authentication
source_filename: bubbles-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bubbles-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token issued in the Bubble app's Settings → API tab.\n  sources:\n  - openapi/bubbles-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bubbles/refs/heads/main/authentication/bubbles-authentication.yml
summary_line: http · 1 scheme
tags:
- Applications
- Low Code
- No Code
- Visual Programming
- Webhooks
- Web Apps
---
