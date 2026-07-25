---
api_key_in: []
api_specs:
- filename: hubilo-event-api-openapi.yml
  format: yaml
  label: hubilo Event API
  slug: hubilo-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/openapi/hubilo-event-api-openapi.yml
- filename: hubilo-exhibitor-api-openapi.yml
  format: yaml
  label: hubilo Exhibitor API
  slug: hubilo-exhibitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/openapi/hubilo-exhibitor-api-openapi.yml
- filename: hubilo-organiser-api-openapi.yml
  format: yaml
  label: hubilo Organiser API
  slug: hubilo-organiser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/openapi/hubilo-organiser-api-openapi.yml
- filename: hubilo-session-api-openapi.yml
  format: yaml
  label: hubilo Session API
  slug: hubilo-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/openapi/hubilo-session-api-openapi.yml
- filename: hubilo-speaker-api-openapi.yml
  format: yaml
  label: hubilo Speaker API
  slug: hubilo-speaker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/openapi/hubilo-speaker-api-openapi.yml
- filename: hubilo-upload-media-api-openapi.yml
  format: yaml
  label: hubilo Upload Media API
  slug: hubilo-upload-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/openapi/hubilo-upload-media-api-openapi.yml
- filename: hubilo-user-api-openapi.yml
  format: yaml
  label: hubilo User API
  slug: hubilo-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/openapi/hubilo-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hubilo Authentication
name_suffix: Authentication
oauth_flows: []
overview: hubilo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: hubilo
provider_slug: hubilo
scheme_count: 1
schemes:
- description: Access Token issued to the organiser, sent in the Authorization header as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hubilo-openapi.yml
  type: http
slug: hubilo-authentication
source_filename: hubilo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hubilo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Access Token issued to the organiser, sent in the Authorization header as a Bearer\n    token.\n  sources:\n  - openapi/hubilo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubilo/refs/heads/main/authentication/hubilo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Events
- Virtual Events
- Webinars
- Event Management
- Hybrid Events
- Attendee Engagement
---
