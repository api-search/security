---
api_key_in: []
api_specs:
- filename: eventbrite-openapi.yml
  format: yaml
  label: Eventbrite Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Eventbrite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eventbrite secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eventbrite
provider_slug: eventbrite
scheme_count: 1
schemes:
- description: OAuth 2.0 token (private token or OAuth-issued)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/eventbrite-openapi.yml
  type: http
slug: eventbrite-authentication
source_filename: eventbrite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eventbrite-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 token (private token or OAuth-issued)\n  sources:\n  - openapi/eventbrite-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/authentication/eventbrite-authentication.yml
summary_line: http · 1 scheme
tags:
- Events
- Event Technology
- Ticketing
- Marketplace
---
