---
api_key_in: []
api_specs:
- filename: spurwing-openapi.yml
  format: yaml
  label: Spurwing Providers API
  slug: providers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spurwing/refs/heads/main/openapi/spurwing-openapi.yml
- filename: spurwing-openapi.yml
  format: yaml
  label: Spurwing Availability API
  slug: availability
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spurwing/refs/heads/main/openapi/spurwing-openapi.yml
- filename: spurwing-openapi.yml
  format: yaml
  label: Spurwing Appointments API
  slug: appointments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spurwing/refs/heads/main/openapi/spurwing-openapi.yml
- filename: spurwing-openapi.yml
  format: yaml
  label: Spurwing Services API
  slug: services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spurwing/refs/heads/main/openapi/spurwing-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Spurwing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spurwing secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spurwing
provider_slug: spurwing
scheme_count: 1
schemes:
- description: Private API key issued on the Spurwing dashboard (API Info page), passed as an Authorization Bearer token. Never expose the API key in front-end code.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/spurwing-openapi.yml
  type: http
slug: spurwing-authentication
source_filename: spurwing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spurwing-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Private API key issued on the Spurwing dashboard (API Info page), passed as an\n    Authorization Bearer token. Never expose the API key in front-end code.\n  sources:\n  - openapi/spurwing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spurwing/refs/heads/main/authentication/spurwing-authentication.yml
summary_line: http · 1 scheme
tags:
- Scheduling
- Appointments
- Booking
- Calendar
- Availability
---
