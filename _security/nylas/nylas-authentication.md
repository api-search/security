---
api_key_in: []
api_specs:
- filename: nylas-openapi.yml
  format: yaml
  label: Nylas API
  slug: nylas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nylas Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nylas secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nylas
provider_slug: nylas
scheme_count: 1
schemes:
- description: 'Server-side requests use an API key issued in the Nylas dashboard

    and presented as a Bearer token. User-level requests use an

    access token obtained via the OAuth 2.0 flow.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/nylas-openapi.yml
  type: http
slug: nylas-authentication
source_filename: nylas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nylas-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Server-side requests use an API key issued in the Nylas dashboard\n    and presented as a Bearer token. User-level requests use an\n    access token obtained via the OAuth 2.0 flow.\n  sources:\n  - openapi/nylas-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/authentication/nylas-authentication.yml
summary_line: http · 1 scheme
tags:
- Calendar
- Communication
- Contacts
- Email
- Messaging
- Scheduling
---
