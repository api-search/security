---
api_key_in:
- header
api_specs:
- filename: mailtrap-email-api-openapi.yml
  format: yaml
  label: Mailtrap Email Sending API
  slug: mailtrap-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailtrap/refs/heads/main/openapi/mailtrap-email-api-openapi.yml
- filename: mailtrap-email-sandbox-openapi.yml
  format: yaml
  label: Mailtrap Email Sandbox API
  slug: mailtrap-email-sandbox
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailtrap/refs/heads/main/openapi/mailtrap-email-sandbox-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mailtrap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mailtrap secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mailtrap
provider_slug: mailtrap
scheme_count: 2
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/mailtrap-email-api-openapi.yml
  type: http
- in: header
  name: ApiTokenAuth
  parameter: Api-Token
  sources:
  - openapi/mailtrap-email-sandbox-openapi.yml
  type: apiKey
slug: mailtrap-authentication
source_filename: mailtrap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mailtrap-email-api-openapi.yml, openapi/mailtrap-email-sandbox-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/mailtrap-email-api-openapi.yml\n- name: ApiTokenAuth\n  type: apiKey\n  in: header\n  parameter: Api-Token\n  sources:\n  - openapi/mailtrap-email-sandbox-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailtrap/refs/heads/main/authentication/mailtrap-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Email
- Email Delivery
- Email Sandbox
- Email Testing
- Transactional Email
---
