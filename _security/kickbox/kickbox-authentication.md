---
api_key_in: []
api_specs:
- filename: kickbox-openapi.yml
  format: yaml
  label: Kickbox Email Verification API
  slug: verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kickbox/refs/heads/main/openapi/kickbox-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kickbox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kickbox secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kickbox
provider_slug: kickbox
scheme_count: 1
schemes:
- bearerFormat: token
  description: 'Kickbox API key sent in the Authorization header in the form

    `Authorization: token YOUR_API_KEY`.'
  name: TokenAuth
  scheme: bearer
  sources:
  - openapi/kickbox-openapi.yml
  type: http
slug: kickbox-authentication
source_filename: kickbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kickbox-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: TokenAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  description: |-\n    Kickbox API key sent in the Authorization header in the form\n    `Authorization: token YOUR_API_KEY`.\n  sources:\n  - openapi/kickbox-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kickbox/refs/heads/main/authentication/kickbox-authentication.yml
summary_line: http · 1 scheme
tags:
- Email Verification
- Email Validation
- Deliverability
- Data Quality
- Email
---
