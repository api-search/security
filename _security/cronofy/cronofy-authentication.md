---
api_key_in: []
api_specs:
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Calendars API
  slug: calendars
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Events API
  slug: events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Availability API
  slug: availability
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Smart Invites API
  slug: smart-invites
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Scheduling Links API
  slug: scheduling-links
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Push Notifications API
  slug: push-notifications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cronofy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cronofy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cronofy
provider_slug: cronofy
scheme_count: 1
schemes:
- description: OAuth 2.0 access token passed as an Authorization Bearer header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cronofy-openapi.yml
  type: http
slug: cronofy-authentication
source_filename: cronofy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cronofy-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token passed as an Authorization Bearer header.\n  sources:\n  - openapi/cronofy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/authentication/cronofy-authentication.yml
summary_line: http · 1 scheme
tags:
- Scheduling
- Calendar
- Availability
- Booking
- Productivity
---
