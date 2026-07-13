---
api_key_in:
- header
api_specs:
- filename: maileroo-email-api-openapi.yml
  format: yaml
  label: Maileroo Email API
  slug: maileroo-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maileroo/refs/heads/main/openapi/maileroo-email-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Maileroo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maileroo secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Maileroo
provider_slug: maileroo
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/maileroo-email-api-openapi.yml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/maileroo-email-api-openapi.yml
  type: http
slug: maileroo-authentication
source_filename: maileroo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/maileroo-email-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/maileroo-email-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/maileroo-email-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maileroo/refs/heads/main/authentication/maileroo-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Email
- Email Delivery
- Marketing Email
- SMTP
- Transactional Email
---
